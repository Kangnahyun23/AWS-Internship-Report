---
title: "Worklog Tuần 5"
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:

* Hiểu về tính sẵn sàng cao (High Availability) và khả năng mở rộng (Scalability).
* Cấu hình EC2 Auto Scaling để tự động tăng/giảm số lượng server.
* Giám sát hệ thống toàn diện với Amazon CloudWatch.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - **Chuẩn bị cho Auto Scaling:**<br>+ Tạo AMI (Amazon Machine Image) từ EC2 Instance đã cấu hình sẵn<br>+ Tạo Launch Template từ AMI đó | 06/10/2025 | 06/10/2025 | Cloud Journey - Auto Scaling |
| 3 | - **Cấu hình Auto Scaling Group (ASG):**<br>+ Tạo ASG sử dụng Launch Template<br>+ Cấu hình Min/Max/Desired capacity<br>+ Tích hợp với Application Load Balancer (ALB) | 07/10/2025 | 07/10/2025 | Cloud Journey - Auto Scaling |
| 4 | - **Amazon CloudWatch (Phần 1):**<br>+ Tìm hiểu về Metrics và Logs<br>+ Xem các chỉ số CPU, Network của EC2 trên CloudWatch Console | 08/10/2025 | 08/10/2025 | Cloud Journey - CloudWatch |
| 5 | - **Amazon CloudWatch (Phần 2) & Scaling Policy:**<br>+ Tạo CloudWatch Alarm cảnh báo khi CPU > 70%<br>+ Cấu hình Dynamic Scaling Policy cho ASG dựa trên Alarm này<br>+ Thực hành Stress Test để kích hoạt Auto Scaling | 09/10/2025 | 09/10/2025 | Cloud Journey - CloudWatch |
| 6 | - **Tổng kết tuần 5:**<br>+ Quan sát quá trình Scale-out và Scale-in<br>+ Tạo CloudWatch Dashboard tổng hợp các chỉ số quan trọng | 10/10/2025 | 10/10/2025 | Self-review |


### Kết quả đạt được tuần 5:

* Xây dựng được hệ thống có khả năng tự phục hồi và mở rộng theo nhu cầu thực tế.
* Hiểu rõ vai trò của Load Balancer trong việc phân phối tải.
* Sử dụng thành thạo CloudWatch để giám sát "sức khỏe" của hệ thống.
* Thực hiện thành công kịch bản Stress Test để kiểm chứng khả năng Auto Scaling.
