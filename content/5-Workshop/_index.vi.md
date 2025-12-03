---
title: "Workshop"
weight: 5
chapter: false
pre: " <b> 5. </b> "
---

# Xây dựng Frontend Serverless với Next.js & AWS Amplify

### Tổng quan Workshop

Chào mừng bạn đến với Workshop **Xây dựng Frontend Serverless hiện đại**. Đây không chỉ là một bài hướng dẫn code, mà là hành trình đúc kết từ kinh nghiệm thực tế để xây dựng một ứng dụng web **Production-Ready**.

Chúng ta sẽ cùng nhau giải quyết bài toán: *Làm thế nào để tạo ra một ứng dụng AI có giao diện đẹp, tốc độ nhanh, bảo mật cao mà không cần quản lý server?*

**Đối tượng phù hợp:**
*   Frontend Developer muốn học thêm về Cloud & DevOps.
*   Sinh viên muốn có một đồ án "xịn sò" với công nghệ mới nhất.
*   Bất kỳ ai yêu thích Next.js và AWS.

### Kiến trúc hệ thống

Thay vì chỉ chạy code trên máy local, chúng ta sẽ xây dựng một hệ thống hoàn chỉnh trên AWS:

![Architecture Diagram](/images/workshop_architecture_diagram_1764662750000.png)

**Luồng dữ liệu (Data Flow):**
1.  **User** truy cập website qua tên miền riêng (Route 53).
2.  Request đi qua **AWS WAF** để lọc bỏ các truy cập độc hại.
3.  **CloudFront (CDN)** trả về nội dung tĩnh (HTML/CSS/JS) ngay lập tức từ Edge Location.
4.  Khi User chat với AI, Request được gửi đến **API Gateway**.
5.  **Cognito** xác thực User (đảm bảo chỉ người đã login mới được chat).
6.  **Lambda** xử lý logic và gọi **RDS Database** để lưu lịch sử.

### Các dịch vụ AWS được sử dụng

| Danh mục | Dịch vụ |
| :--- | :--- |
| **Compute** | AWS Lambda |
| **Frontend & Hosting** | AWS Amplify Hosting |
| **Authentication** | Amazon Cognito |
| **API** | Amazon API Gateway |
| **Database** | Amazon RDS (PostgreSQL) |
| **Security** | AWS WAF |
| **CDN & DNS** | Amazon CloudFront, Amazon Route 53 |
| **Monitoring** | Amazon CloudWatch, AWS X-Ray |

### Thời gian & Chi phí ước tính

| Mục | Chi tiết |
| :--- | :--- |
| **Thời gian** | 2-3 giờ |
| **Cấp độ** | Trung cấp (Intermediate) |
| **Chi phí** | ~$5-10 (Nếu dọn dẹp sau workshop) |

### Nội dung thực hành

Workshop được chia thành 7 phần, đi từ cơ bản đến nâng cao:

1.  [**Chuẩn bị môi trường:**](5.1-preparation/) Thiết lập VS Code chuẩn chỉ như Senior Dev.
2.  [**UI Implementation:**](5.2-ui-implementation/) Code giao diện "Mystical" với TailwindCSS.
3.  [**Integration:**](5.3-integration/) Kết nối API bảo mật với Custom Hooks.
4.  [**CI/CD Pipeline:**](5.4-deployment/) Deploy tự động, không còn cảnh copy file thủ công.
5.  [**Advanced Deployment:**](5.5-advanced-deployment/) Tối ưu hiệu năng và bảo mật (WAF, CDN).
6.  [**Backend Architecture:**](5.6-backend-architecture/) Hiểu về hệ thống phía sau (VPC, RDS).
7.  [**Cleanup:**](5.7-cleanup/) Dọn dẹp để không mất tiền oan.

---
{{% notice tip %}}
**Lời khuyên:** Đừng chỉ copy-paste code. Hãy đọc kỹ phần **"Chuyện nghề" (My Experience)** ở cuối mỗi bài để tránh những lỗi sai mà mình đã từng mất hàng giờ để debug!
{{% /notice %}}