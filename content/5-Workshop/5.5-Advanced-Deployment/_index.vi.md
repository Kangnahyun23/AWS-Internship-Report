---
title: "Tối ưu hóa, Bảo mật & Giám sát"
weight: 5
chapter: false
pre: " <b> 5.5. </b> "
---

### 1. AWS WAF (Web Application Firewall)

Bảo vệ ứng dụng khỏi các cuộc tấn công web phổ biến như SQL Injection, XSS, và DDoS.

![WAF Security Diagram](/images/waf_security_diagram_1764662992832.png)

**Cấu hình Rate Limiting:**
Để chống DDoS tầng ứng dụng, hãy thiết lập quy tắc giới hạn số lượng request:
*   **Rule Type:** Rate-based rule.
*   **Rate Limit:** 100 requests / 5 minutes.
*   **Action:** Block.
*   **Scope:** Source IP address.

### 2. Amazon CloudFront (CDN)

*   **Caching:** Lưu trữ các file tĩnh tại Edge Location.
*   **Invalidation:** Khi deploy phiên bản mới, Amplify tự động xóa cache cũ.

### 3. Amazon Route 53 (Custom Domain)

Thay vì sử dụng tên miền mặc định dài ngoằng của Amplify (`...amplifyapp.com`), hãy cấu hình tên miền riêng chuyên nghiệp.

1.  Mua tên miền trên **Route 53**.
2.  Trong Amplify Console > **Domain management** > **Add domain**.
3.  Amplify sẽ tự động tạo bản ghi CNAME và cấp phát chứng chỉ SSL.

### 4. Observability: CloudWatch & X-Ray

**Amazon CloudWatch (Logs & Metrics):**
Theo dõi các chỉ số như CPU, Memory, Request count, và Error Rate.

**AWS X-Ray (Distributed Tracing):**
Giúp bạn nhìn thấy toàn bộ hành trình của một Request: Từ Frontend -> API Gateway -> Lambda -> Database.

---

### Chuyện nghề (My Experience)

{{% notice tip %}}
**Tiết kiệm chi phí CloudWatch**
Mặc định, CloudWatch Logs được lưu trữ **vĩnh viễn** (Never Expire). Điều này sẽ ngốn tiền của bạn sau vài tháng.
**Giải pháp:** Luôn set **Retention Policy** (thời gian lưu trữ) là **1 tuần** hoặc **1 tháng** cho các môi trường Dev/Staging. Chỉ giữ log Production lâu hơn nếu cần Audit.
{{% /notice %}}

### Kiểm thử & Xác thực (Verification)

**Test Case 1: Kiểm tra WAF (Rate Limiting)**
1.  Dùng tool (như JMeter hoặc script Python) gửi liên tục 200 request trong 1 phút đến trang web.
2.  *Kết quả mong đợi:* Sau khoảng 100 request đầu tiên, các request sau sẽ nhận được lỗi **403 Forbidden**.

**Test Case 2: Kiểm tra Domain & SSL**
1.  Truy cập `https://your-domain.com`.
2.  Click vào biểu tượng ổ khóa trên thanh địa chỉ.
3.  *Kết quả mong đợi:* "Connection is secure". Certificate được cấp bởi Amazon.
