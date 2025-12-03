---
title: "Worklog Tuần 2"
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu tuần 2:

* Xây dựng hạ tầng mạng ảo cơ bản (VPC).
* Khởi tạo và quản lý máy chủ ảo (EC2).
* Hiểu về cơ chế cấp quyền cho ứng dụng (IAM Roles).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - **Kiến thức cơ bản về mạng (VPC):**<br>+ Tạo VPC, Subnet (Public/Private)<br>+ Cấu hình Internet Gateway và Route Table | 15/09/2025 | 15/09/2025 | Cloud Journey - VPC |
| 3 | - **Máy chủ ảo EC2 (Phần 1):**<br>+ Tìm hiểu các dòng Instance (Family, Type)<br>+ Tạo Key Pair để kết nối SSH<br>+ Launch EC2 Instance đầu tiên trong Public Subnet | 16/09/2025 | 16/09/2025 | Cloud Journey - EC2 |
| 4 | - **Máy chủ ảo EC2 (Phần 2):**<br>+ Thực hành kết nối SSH vào EC2 (Linux/Windows)<br>+ Tìm hiểu Security Group (Inbound/Outbound rules)<br>+ Cài đặt Web Server (Apache/Nginx) thử nghiệm | 17/09/2025 | 17/09/2025 | Cloud Journey - EC2 |
| 5 | - **Cấp quyền ứng dụng với IAM Roles:**<br>+ Tạo IAM Role cho EC2 (ví dụ: quyền truy cập S3)<br>+ Gán Role vào EC2 Instance đang chạy<br>+ Kiểm tra quyền truy cập từ trong OS | 18/09/2025 | 18/09/2025 | Cloud Journey - IAM Roles |
| 6 | - **Tổng kết tuần 2:**<br>+ Dọn dẹp tài nguyên (Terminate Instance) nếu không dùng<br>+ Ôn tập kiến thức VPC và Security Group | 19/09/2025 | 19/09/2025 | Self-review |


### Kết quả đạt được tuần 2:

* Tự xây dựng được một mạng VPC hoàn chỉnh với khả năng kết nối Internet.
* Thành thạo việc khởi tạo, kết nối và quản lý vòng đời của EC2 Instance.
* Hiểu sâu về Security Group - firewall ảo của AWS.
* Biết cách sử dụng IAM Role để cấp quyền bảo mật cho ứng dụng thay vì dùng Access Key cứng.
