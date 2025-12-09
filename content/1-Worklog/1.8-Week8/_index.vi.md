---
title: "Worklog Tuần 8"
date: 2025-10-31
draft: false
weight: 8
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8
*   Bắt đầu giai đoạn Tối ưu hệ thống (Optimize System).
*   Tự động hóa vận hành (Operations) với AWS Lambda và Systems Manager.
*   Quản lý hạ tầng dưới dạng mã (IaC) cơ bản.
*   **Hoàn thành kỳ thi Giữa kỳ (Midterm Exam).**

### Các công việc cần triển khai trong tuần này

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :--- | :--- | :--- |
| 2 | **Tự động hóa với AWS Lambda:**<br>- Tìm hiểu về Serverless và Lambda function<br>- Viết function Python (Boto3) để tự động Start/Stop EC2 instance theo lịch<br>- Cấu hình EventBridge (CloudWatch Events) để kích hoạt Lambda<br><br>**Dự án SorcererXtreme:**<br>- **RAG Research:**<br>+ Nghiên cứu RAG Flow (Retrieval-Augmented Generation)<br>+ Chọn Model: Amazon Titan Embeddings v2 | 27/10/2025 | 27/10/2025 | [Cloud Journey - Optimize](https://cloudjourney.awsstudygroup.com/) |
| 3 | **Giám sát nâng cao (Observability):**<br>- Tạo Dashboard tùy chỉnh trên CloudWatch<br>- Tích hợp CloudWatch với SNS để gửi cảnh báo qua Email/SMS<br>- Tìm hiểu về Grafana (nếu có trong chương trình)<br><br>**Dự án SorcererXtreme:**<br>- **Data Prep:**<br>+ Chuẩn bị dữ liệu Tarot/Chiêm tinh (Text/JSON)<br>+ Viết script Chunking dữ liệu | 28/10/2025 | 28/10/2025 | [Cloud Journey - Optimize](https://cloudjourney.awsstudygroup.com/) |
| 4 | **AWS Systems Manager (SSM):**<br>- Cài đặt SSM Agent lên EC2<br>- Sử dụng Session Manager để remote vào EC2 không cần mở port 22 (SSH)<br>- Sử dụng Run Command để chạy lệnh trên nhiều server cùng lúc<br><br>**Dự án SorcererXtreme:**<br>- **Vector DB:**<br>+ Viết Lambda function tạo Vector từ Text<br>+ Lưu trữ Vector vào Pinecone | 29/10/2025 | 29/10/2025 | [Cloud Journey - Optimize](https://cloudjourney.awsstudygroup.com/) |
| 5 | **Quản lý tài nguyên & IaC:**<br>- Sử dụng Tagging Strategy để quản lý chi phí và tài nguyên<br>- Tìm hiểu AWS CloudFormation cơ bản<br>- Tạo một Stack đơn giản (ví dụ: tạo S3 bucket bằng code YAML/JSON)<br><br>**Ôn tập tổng hợp trước thi:**<br>- Review lại AWS Well-Architected Framework<br>- Hệ thống hóa lại các dịch vụ trọng tâm: EC2, S3, IAM, RDS, VPC...<br><br>**Dự án SorcererXtreme:**<br>- **Test Search:**<br>+ Test khả năng Semantic Search với Pinecone | 30/10/2025 | 30/10/2025 | [Cloud Journey - Optimize](https://cloudjourney.awsstudygroup.com/)<br>Midterm Revision |
| 6 | **THI GIỮA KỲ (MIDTERM EXAM):**<br>- **Thời gian:** 31/10/2025 (90 phút)<br>- **Địa điểm:** Văn phòng AWS - Tầng 26, Bitexco Financial Tower<br>- **Nội dung:** Secure, Resilient, High-Performing, Cost-Optimized Architectures<br>- **Hình thức:** Trắc nghiệm online | 31/10/2025 | 31/10/2025 | **Midterm Exam** |

### Kết quả đạt được tuần 8
*   Bước đầu tiếp cận tư duy "Automate everything" trong vận hành hệ thống.
*   Viết được Lambda function thực tế giúp tiết kiệm chi phí (tắt server giờ nghỉ).
*   Quản lý server an toàn và chuyên nghiệp hơn với Systems Manager (không cần Bastion Host).
*   Hiểu khái niệm Infrastructure as Code (IaC) để chuẩn bị cho các bài toán triển khai lớn.
*   Hoàn thành bài thi đánh giá năng lực giữa kỳ.
* **Dự án SorcererXtreme:**
    * Nắm vững quy trình RAG (Retrieval-Augmented Generation).
    * Xây dựng Lambda function để chuyển đổi dữ liệu văn bản thành Vector và lưu trữ vào Pinecone.
