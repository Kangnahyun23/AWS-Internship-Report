---
title: "Worklog Tuần 7"
date: 2025-10-24
draft: false
weight: 7
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7
*   Nâng cao kiến thức về mạng AWS (Networking Advanced).
*   Tối ưu hóa phân phối nội dung với CDN (CloudFront).
*   Bảo mật ứng dụng web ở tầng biên (Edge Security).

### Các công việc cần triển khai trong tuần này

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :--- | :--- | :--- |
| 2 | **Workshop về mạng (Phần 1):**<br>- Tìm hiểu về VPC Peering (kết nối 2 VPC)<br>- Thực hành tạo 2 VPC và thiết lập Peering Connection<br>- Cấu hình Route Table để 2 VPC thông nhau<br><br>**Dự án SorcererXtreme:**<br>- **UI Design:**<br>+ Xây dựng Global Layout & Sidebar (Glassmorphism)<br>+ Responsive Design cho Mobile/Tablet | 20/10/2025 | 20/10/2025 | [Cloud Journey - Networking](https://cloudjourney.awsstudygroup.com/) |
| 3 | **Workshop về mạng (Phần 2):**<br>- Tìm hiểu về Site-to-Site VPN (lý thuyết)<br>- Thực hành giả lập kết nối VPN (nếu có điều kiện) hoặc tìm hiểu Transit Gateway<br>- VPC Endpoints (PrivateLink) để truy cập dịch vụ AWS nội bộ<br><br>**Dự án SorcererXtreme:**<br>- **Frontend Dev:**<br>+ Xây dựng `ChatComponent`: Bong bóng tin nhắn, Input<br>+ Thêm Animation (Framer Motion) | 21/10/2025 | 21/10/2025 | [Cloud Journey - Networking](https://cloudjourney.awsstudygroup.com/) |
| 4 | **Amazon CloudFront (Phần 1):**<br>- Tìm hiểu về CDN và Edge Locations<br>- Tạo CloudFront Distribution cho S3 Bucket (đã làm tuần 3)<br>- Cấu hình OAI (Origin Access Identity) để bảo mật S3<br><br>**Dự án SorcererXtreme:**<br>- **Cognito Backend:**<br>+ Cấu hình `amplify/auth.ts`<br>+ Định nghĩa Email/Password login | 22/10/2025 | 22/10/2025 | [Cloud Journey - CloudFront](https://cloudjourney.awsstudygroup.com/) |
| 5 | **Amazon CloudFront (Phần 2) & WAF:**<br>- Cấu hình Custom Domain và SSL Certificate (ACM) cho CloudFront<br>- Tìm hiểu AWS WAF (Web Application Firewall)<br>- Tạo WAF ACL đơn giản chặn IP hoặc Geo-blocking gắn vào CloudFront<br><br>**Ôn tập thi Giữa kỳ (Phần 1):**<br>- Thiết kế kiến trúc bảo mật (IAM, MFA, SCP, Encryption, Security Groups, WAF...)<br>- Thiết kế kiến trúc linh hoạt (Multi-AZ, Auto Scaling, Route 53...)<br><br>**Dự án SorcererXtreme:**<br>- **Auth Frontend:**<br>+ Tạo trang Login/Register với Amplify UI<br>+ Custom Theme form đăng nhập | 23/10/2025 | 23/10/2025 | [Cloud Journey - CloudFront](https://cloudjourney.awsstudygroup.com/)<br>Midterm Revision |
| 6 | **Tổng kết tuần 7 & Ôn tập:**<br>- Kiểm tra tốc độ truy cập website qua CDN so với trực tiếp S3<br>- Review lại toàn bộ kiến thức về Networking và Content Delivery<br><br>**Ôn tập thi Giữa kỳ (Phần 2):**<br>- Thiết kế hệ thống hiệu năng cao (EC2 Auto Scaling, Lambda, S3, Caching...)<br>- Thiết kế tối ưu chi phí (Cost Explorer, Savings Plans, Storage Tiering...) | 24/10/2025 | 24/10/2025 | Self-review<br>Midterm Revision |

### Kết quả đạt được tuần 7
*   Hiểu sâu về kiến trúc mạng trong AWS, cách kết nối các VPC với nhau.
*   Triển khai thành công CDN giúp tăng tốc độ tải trang cho người dùng toàn cầu.
*   Biết cách bảo mật nội dung gốc (S3) không cho truy cập trực tiếp.
*   Nắm được cách bảo vệ ứng dụng khỏi các cuộc tấn công web cơ bản với WAF.
* **Dự án SorcererXtreme:**
    * Hoàn thiện giao diện Chat UI theo phong cách Mystical/Glassmorphism.
    * Tích hợp thành công hệ thống xác thực người dùng (Auth) với Amazon Cognito.
