---
title: "Worklog Tuần 9"
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu tuần 9:

* Bắt đầu giai đoạn Hiện đại hóa ứng dụng (Modernize Application).
* Tìm hiểu về kiến trúc Serverless.
* Xây dựng API đầu tiên với API Gateway và Lambda.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - **Serverless Overview:**<br>+ Tìm hiểu khái niệm Serverless và lợi ích<br>+ Phân tích kiến trúc Monolith vs Microservices<br>+ Giới thiệu bộ ba: Lambda, API Gateway, DynamoDB | 03/11/2025 | 03/11/2025 | [Cloud Journey - Modernize](https://cloudjourney.awsstudygroup.com/) |
| 3 | - **AWS Lambda & DynamoDB:**<br>+ Viết Lambda function (Node.js/Python) để tương tác với DynamoDB (CRUD)<br>+ Cấu hình IAM Role cho phép Lambda truy cập DynamoDB | 04/11/2025 | 04/11/2025 | [Cloud Journey - Serverless](https://cloudjourney.awsstudygroup.com/) |
| 4 | - **Amazon API Gateway:**<br>+ Tạo REST API với API Gateway<br>+ Tích hợp API Gateway với Lambda function<br>+ Deploy API và test bằng Postman | 05/11/2025 | 05/11/2025 | [Cloud Journey - Serverless](https://cloudjourney.awsstudygroup.com/) |
| 5 | - **Xây dựng Backend Serverless:**<br>+ Hoàn thiện các API: Create, Read, Update, Delete Item<br>+ Xử lý lỗi (Error Handling) và phản hồi (Response Mapping) trong Lambda | 06/11/2025 | 06/11/2025 | [Cloud Journey - Serverless](https://cloudjourney.awsstudygroup.com/) |
| 6 | - **Tổng kết tuần 9:**<br>+ Review kiến trúc Serverless đã xây dựng<br>+ So sánh chi phí và hiệu năng so với chạy trên EC2 truyền thống | 07/11/2025 | 07/11/2025 | Self-review |


### Kết quả đạt được tuần 9:

* Hiểu rõ tư duy thiết kế ứng dụng theo hướng Serverless (không quản lý máy chủ).
* Xây dựng thành công hệ thống Backend hoàn chỉnh (API + Compute + Database) mà không cần khởi tạo bất kỳ server nào.
* Nắm vững cách tích hợp giữa các dịch vụ cốt lõi: API Gateway -> Lambda -> DynamoDB.
