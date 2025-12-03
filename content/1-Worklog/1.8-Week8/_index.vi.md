---
title: "Worklog Tuần 8"
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8:

* Bắt đầu giai đoạn Tối ưu hệ thống (Optimize System).
* Tự động hóa vận hành (Operations) với AWS Lambda và Systems Manager.
* Quản lý hạ tầng dưới dạng mã (IaC) cơ bản.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - **Tự động hóa với AWS Lambda:**<br>+ Tìm hiểu về Serverless và Lambda function<br>+ Viết function Python (Boto3) để tự động Start/Stop EC2 instance theo lịch<br>+ Cấu hình EventBridge (CloudWatch Events) để kích hoạt Lambda | 27/10/2025 | 27/10/2025 | Cloud Journey - Optimize |
| 3 | - **Giám sát nâng cao (Observability):**<br>+ Tạo Dashboard tùy chỉnh trên CloudWatch<br>+ Tích hợp CloudWatch với SNS để gửi cảnh báo qua Email/SMS<br>+ Tìm hiểu về Grafana (nếu có trong chương trình) | 28/10/2025 | 28/10/2025 | Cloud Journey - Optimize |
| 4 | - **AWS Systems Manager (SSM):**<br>+ Cài đặt SSM Agent lên EC2<br>+ Sử dụng Session Manager để remote vào EC2 không cần mở port 22 (SSH)<br>+ Sử dụng Run Command để chạy lệnh trên nhiều server cùng lúc | 29/10/2025 | 29/10/2025 | Cloud Journey - Optimize |
| 5 | - **Quản lý tài nguyên & IaC:**<br>+ Sử dụng Tagging Strategy để quản lý chi phí và tài nguyên<br>+ Tìm hiểu AWS CloudFormation cơ bản<br>+ Tạo một Stack đơn giản (ví dụ: tạo S3 bucket bằng code YAML/JSON) | 30/10/2025 | 30/10/2025 | Cloud Journey - Optimize |
| 6 | - **Tổng kết tuần 8:**<br>+ Review các giải pháp tự động hóa đã triển khai<br>+ Đánh giá hiệu quả của việc dùng SSM so với SSH truyền thống | 31/10/2025 | 31/10/2025 | Self-review |


### Kết quả đạt được tuần 8:

* Bước đầu tiếp cận tư duy "Automate everything" trong vận hành hệ thống.
* Viết được Lambda function thực tế giúp tiết kiệm chi phí (tắt server giờ nghỉ).
* Quản lý server an toàn và chuyên nghiệp hơn với Systems Manager (không cần Bastion Host).
* Hiểu khái niệm Infrastructure as Code (IaC) để chuẩn bị cho các bài toán triển khai lớn.
