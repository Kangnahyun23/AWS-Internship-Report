---
title: "Kiến trúc Backend tham khảo (RDS & VPC)"
weight: 6
chapter: false
pre: " <b> 5.6. </b> "
---

### 1. Mô hình kiến trúc VPC

Backend được triển khai trong một **VPC (Virtual Private Cloud)** để đảm bảo an toàn tối đa:

![VPC Architecture Diagram](/images/vpc_rds_architecture_1764663010653.png)

*   **Public Subnet:** Chứa **NAT Gateway** (để server nội bộ truy cập Internet) và **Bastion Host**.
*   **Private Subnet (App Layer):** Chứa **AWS Lambda**.
*   **Private Subnet (Data Layer):** Chứa **Amazon RDS (PostgreSQL)**.

### 2. Cấu hình Security Group (Firewall)

Để đảm bảo nguyên tắc "Least Privilege" (Quyền tối thiểu), chúng ta thiết lập các quy tắc Security Group chặt chẽ:

| Security Group | Inbound Rule | Outbound Rule | Mô tả |
| :--- | :--- | :--- | :--- |
| **SG-Lambda** | None (hoặc từ API Gateway nếu cần) | Allow All to **SG-RDS** (Port 5432) | Lambda chỉ được phép gọi vào Database. |
| **SG-RDS** | Allow TCP 5432 from **SG-Lambda** | None | Database chỉ chấp nhận kết nối từ Lambda, từ chối mọi nguồn khác. |

### 3. VPC Endpoints (PrivateLink)

Để Lambda truy cập các dịch vụ AWS khác (như S3, Secrets Manager, CloudWatch) mà không cần đi ra Internet công cộng (qua NAT Gateway), hãy sử dụng **VPC Endpoints**.

---

### Chuyện nghề (My Experience)

{{% notice warning %}}
**Tại sao không để Database ở Public Subnet?**
Nhiều bạn mới học thường để RDS ở Public Subnet cho dễ kết nối từ máy tính cá nhân. **Đừng bao giờ làm thế ở Production!** Hacker có thể brute-force mật khẩu của bạn.
**Giải pháp:** Luôn để RDS ở Private Subnet. Nếu muốn kết nối từ máy local để debug, hãy dùng **Bastion Host** (nhảy cầu) hoặc **AWS VPN Client**.
{{% /notice %}}

### Kiểm thử & Xác thực (Verification)

**Test Case 1: Kiểm tra kết nối Lambda -> RDS**
1.  Tạo một Lambda function đơn giản thực hiện query `SELECT NOW();`.
2.  Gán Lambda vào Private Subnet và SG-Lambda.
3.  Chạy Test trên AWS Console.
4.  *Kết quả mong đợi:* Trả về thời gian hiện tại của Database.

**Test Case 2: Kiểm tra chặn truy cập ngoài**
1.  Thử kết nối trực tiếp đến Endpoint của RDS từ máy tính cá nhân (qua Internet).
2.  *Kết quả mong đợi:* **Connection Timeout** (Không thể kết nối). Điều này chứng tỏ Database đã được bảo vệ an toàn trong VPC.
