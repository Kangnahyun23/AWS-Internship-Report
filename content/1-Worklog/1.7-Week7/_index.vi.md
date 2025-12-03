---
title: "Worklog Tuần 7"
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

* Nâng cao kiến thức về mạng AWS (Networking Advanced).
* Tối ưu hóa phân phối nội dung với CDN (CloudFront).
* Bảo mật ứng dụng web ở tầng biên (Edge Security).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - **Workshop về mạng (Phần 1):**<br>+ Tìm hiểu về VPC Peering (kết nối 2 VPC)<br>+ Thực hành tạo 2 VPC và thiết lập Peering Connection<br>+ Cấu hình Route Table để 2 VPC thông nhau | 20/10/2025 | 20/10/2025 | Cloud Journey - Networking |
| 3 | - **Workshop về mạng (Phần 2):**<br>+ Tìm hiểu về Site-to-Site VPN (lý thuyết)<br>+ Thực hành giả lập kết nối VPN (nếu có điều kiện) hoặc tìm hiểu Transit Gateway<br>+ VPC Endpoints (PrivateLink) để truy cập dịch vụ AWS nội bộ | 21/10/2025 | 21/10/2025 | Cloud Journey - Networking |
| 4 | - **Amazon CloudFront (Phần 1):**<br>+ Tìm hiểu về CDN và Edge Locations<br>+ Tạo CloudFront Distribution cho S3 Bucket (đã làm tuần 3)<br>+ Cấu hình OAI (Origin Access Identity) để bảo mật S3 | 22/10/2025 | 22/10/2025 | Cloud Journey - CloudFront |
| 5 | - **Amazon CloudFront (Phần 2) & WAF:**<br>+ Cấu hình Custom Domain và SSL Certificate (ACM) cho CloudFront<br>+ Tìm hiểu AWS WAF (Web Application Firewall)<br>+ Tạo WAF ACL đơn giản chặn IP hoặc Geo-blocking gắn vào CloudFront | 23/10/2025 | 23/10/2025 | Cloud Journey - CloudFront |
| 6 | - **Tổng kết tuần 7:**<br>+ Kiểm tra tốc độ truy cập website qua CDN so với trực tiếp S3<br>+ Review lại toàn bộ kiến thức về Networking và Content Delivery | 24/10/2025 | 24/10/2025 | Self-review |


### Kết quả đạt được tuần 7:

* Hiểu sâu về kiến trúc mạng trong AWS, cách kết nối các VPC với nhau.
* Triển khai thành công CDN giúp tăng tốc độ tải trang cho người dùng toàn cầu.
* Biết cách bảo mật nội dung gốc (S3) không cho truy cập trực tiếp.
* Nắm được cách bảo vệ ứng dụng khỏi các cuộc tấn công web cơ bản với WAF.
