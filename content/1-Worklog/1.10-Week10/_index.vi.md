---
title: "Worklog Tuần 10"
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu tuần 10:

* Hoàn thiện ứng dụng Serverless (Frontend + Backend).
* Bảo mật ứng dụng với Amazon Cognito.
* Xử lý bất đồng bộ với SQS/SNS.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - **Frontend Serverless:**<br>+ Xây dựng trang web tĩnh (HTML/JS) gọi API Gateway<br>+ Host trang web trên S3 với SSL (HTTPS)<br>+ Xử lý CORS trên API Gateway | 10/11/2025 | 10/11/2025 | [Cloud Journey - Serverless](https://cloudjourney.awsstudygroup.com/) |
| 3 | - **Xác thực với Amazon Cognito:**<br>+ Tạo User Pool để quản lý người dùng<br>+ Tích hợp Cognito vào Frontend (Đăng ký/Đăng nhập)<br>+ Bảo vệ API Gateway bằng Cognito Authorizer | 11/11/2025 | 11/11/2025 | [Cloud Journey - Cognito](https://cloudjourney.awsstudygroup.com/) |
| 4 | - **Messaging & Eventing:**<br>+ Tìm hiểu về Decoupling architecture<br>+ Tạo SQS Queue để nhận đơn hàng chờ xử lý<br>+ Tạo SNS Topic để gửi thông báo email | 12/11/2025 | 12/11/2025 | [Cloud Journey - SQS/SNS](https://cloudjourney.awsstudygroup.com/) |
| 5 | - **Tích hợp hệ thống:**<br>+ Sửa Lambda để đẩy message vào SQS thay vì xử lý ngay<br>+ Viết Lambda Trigger để xử lý message từ SQS<br>+ Gửi thông báo qua SNS khi xử lý xong | 13/11/2025 | 13/11/2025 | [Cloud Journey - Serverless](https://cloudjourney.awsstudygroup.com/) |
| 6 | - **Tổng kết tuần 10:**<br>+ Test toàn bộ luồng: Frontend -> API -> Lambda -> SQS -> Lambda -> DB -> SNS<br>+ Đánh giá độ trễ và khả năng chịu tải | 14/11/2025 | 14/11/2025 | Self-review |


### Kết quả đạt được tuần 10:

* Xây dựng thành công ứng dụng Fullstack Serverless hoàn chỉnh.
* Biết cách bảo mật API và quản lý người dùng chuyên nghiệp với Cognito.
* Hiểu và triển khai được kiến trúc xử lý bất đồng bộ (Asynchronous) giúp hệ thống không bị nghẽn cổ chai.
