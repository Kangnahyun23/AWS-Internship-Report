---
title: "Worklog Tuần 6"
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:

* Làm quen với cơ sở dữ liệu NoSQL (DynamoDB).
* Tìm hiểu về Caching để tăng tốc độ ứng dụng (ElastiCache).
* Nâng cao kỹ năng sử dụng AWS CLI.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - **Amazon DynamoDB (Phần 1):**<br>+ Tìm hiểu sự khác biệt giữa SQL (RDS) và NoSQL (DynamoDB)<br>+ Tạo bảng DynamoDB (Partition Key, Sort Key)<br><br>**Dự án SorcererXtreme:**<br>- **Khởi tạo Project:**<br>+ Tạo Next.js 14 App (TypeScript, Tailwind CSS)<br>+ Cài đặt thư viện: `framer-motion`, `lucide-react` | 13/10/2025 | 13/10/2025 | [Cloud Journey - DynamoDB](https://cloudjourney.awsstudygroup.com/) |
| 3 | - **Amazon DynamoDB (Phần 2):**<br>+ Thực hành thêm, sửa, xóa (CRUD) item trên Console<br>+ Tìm hiểu về Read/Write Capacity Units (RCU/WCU)<br><br>**Dự án SorcererXtreme:**<br>- **Setup Amplify Gen 2:**<br>+ Chạy `npm create amplify@latest`<br>+ Deploy môi trường Sandbox | 14/10/2025 | 14/10/2025 | [Cloud Journey - DynamoDB](https://cloudjourney.awsstudygroup.com/) |
| 4 | - **Amazon ElastiCache:**<br>+ Tìm hiểu về In-memory Caching (Redis/Memcached)<br>+ Khởi tạo ElastiCache Redis Cluster<br>+ Kết nối thử từ EC2 vào Redis<br><br>**Dự án SorcererXtreme:**<br>- **Setup Database:**<br>+ Tạo tài khoản NeonDB (SQL) cho RAG<br>+ Tạo Index trên Pinecone (Vector DB) | 15/10/2025 | 15/10/2025 | [Cloud Journey - ElastiCache](https://cloudjourney.awsstudygroup.com/) |
| 5 | - **AWS CLI Nâng cao:**<br>+ Sử dụng AWS CLI để tương tác với DynamoDB (put-item, get-item)<br>+ Viết script bash đơn giản để backup dữ liệu từ S3 hoặc DynamoDB<br><br>**Dự án SorcererXtreme:**<br>- **Setup CI/CD:**<br>+ Push code lên GitHub<br>+ Kết nối Amplify Console để kích hoạt Pipeline | 16/10/2025 | 16/10/2025 | [Cloud Journey - AWS CLI](https://cloudjourney.awsstudygroup.com/) |
| 6 | - **Tổng kết tuần 6:**<br>+ Review kiến thức về Database (SQL vs NoSQL vs Cache)<br>+ Hoàn thiện báo cáo giữa kỳ (nếu có) | 17/10/2025 | 17/10/2025 | Self-review |


### Kết quả đạt được tuần 6:

* Hiểu rõ mô hình dữ liệu NoSQL và cách thiết kế bảng đơn giản trong DynamoDB.
* Biết cách sử dụng Caching để giảm tải cho Database chính.
* Thành thạo hơn trong việc sử dụng công cụ dòng lệnh (CLI) để quản trị tài nguyên.
* Có cái nhìn tổng quan về các giải pháp lưu trữ dữ liệu đa dạng trên AWS.
* **Dự án SorcererXtreme:**
    * Khởi tạo thành công dự án với Next.js 14 và Tailwind CSS.
    * Thiết lập môi trường phát triển đám mây với AWS Amplify Gen 2.
    * Chuẩn bị sẵn sàng cơ sở dữ liệu NeonDB (SQL) và Pinecone (Vector) cho tính năng RAG.
