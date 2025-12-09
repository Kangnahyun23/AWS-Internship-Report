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
| 2 | - **Frontend Serverless:**<br>+ Xây dựng trang web tĩnh (HTML/JS) gọi API Gateway<br>+ Host trang web trên S3 với SSL (HTTPS)<br>+ Xử lý CORS trên API Gateway<br><br>**Dự án SorcererXtreme:**<br>- **Frontend Integration:**<br>+ Kết nối Chat UI với Lambda Backend qua API Gateway<br>+ Xử lý CORS và Authentication Token | 10/11/2025 | 10/11/2025 | [Cloud Journey - Serverless](https://cloudjourney.awsstudygroup.com/) |
| 3 | - **Xác thực với Amazon Cognito:**<br>+ Tạo User Pool để quản lý người dùng<br>+ Tích hợp Cognito vào Frontend (Đăng ký/Đăng nhập)<br>+ Bảo vệ API Gateway bằng Cognito Authorizer<br><br>**Dự án SorcererXtreme:**<br>- **UX Improvement:**<br>+ Thêm Loading Skeletons khi chờ phản hồi<br>+ Xử lý lỗi (Error Boundary) và thông báo Toast | 11/11/2025 | 11/11/2025 | [Cloud Journey - Cognito](https://cloudjourney.awsstudygroup.com/) |
| 4 | - **Messaging & Eventing:**<br>+ Tìm hiểu về Decoupling architecture<br>+ Tạo SQS Queue để nhận đơn hàng chờ xử lý<br>+ Tạo SNS Topic để gửi thông báo email<br><br>**Dự án SorcererXtreme:**<br>- **Cost Optimization:**<br>+ Thiết lập AWS Budget cảnh báo chi phí<br>+ Review DynamoDB RCU/WCU (On-demand mode) | 12/11/2025 | 12/11/2025 | [Cloud Journey - SQS/SNS](https://cloudjourney.awsstudygroup.com/) |
| 5 | - **Tích hợp hệ thống:**<br>+ Sửa Lambda để đẩy message vào SQS thay vì xử lý ngay<br>+ Viết Lambda Trigger để xử lý message từ SQS<br>+ Gửi thông báo qua SNS khi xử lý xong<br><br>**Dự án SorcererXtreme:**<br>- **Performance Tuning:**<br>+ Tối ưu Cold Start Lambda (Provisioned Concurrency nếu cần)<br>+ Đo điểm Lighthouse và tối ưu Web Vitals | 13/11/2025 | 13/11/2025 | [Cloud Journey - Serverless](https://cloudjourney.awsstudygroup.com/) |
| 6 | - **Tổng kết tuần 10:**<br>+ Test toàn bộ luồng: Frontend -> API -> Lambda -> SQS -> Lambda -> DB -> SNS<br>+ Đánh giá độ trễ và khả năng chịu tải | 14/11/2025 | 14/11/2025 | Self-review |


### Kết quả đạt được tuần 10:

* Xây dựng thành công ứng dụng Fullstack Serverless hoàn chỉnh.
* Biết cách bảo mật API và quản lý người dùng chuyên nghiệp với Cognito.
* Hiểu và triển khai được kiến trúc xử lý bất đồng bộ (Asynchronous) giúp hệ thống không bị nghẽn cổ chai.
* **Dự án SorcererXtreme:**
    * Kết nối hoàn chỉnh Frontend và Backend, ứng dụng hoạt động trơn tru.
    * Tối ưu hóa trải nghiệm người dùng (UX) và thiết lập kiểm soát chi phí hạ tầng.
