---
title: "Worklog Tuần 11"
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu tuần 11:

* Tự động hóa quy trình triển khai (CI/CD) cho ứng dụng Serverless.
* Giám sát và gỡ lỗi chuyên sâu (Monitoring & Tracing).
* Tìm hiểu về GraphQL (AppSync) - công nghệ API hiện đại.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - **CI/CD với AWS CodePipeline:**<br>+ Tạo Repository trên AWS CodeCommit (hoặc GitHub)<br>+ Tạo Build Project với AWS CodeBuild (buildspec.yml)<br>+ Thiết lập Pipeline tự động deploy khi có code mới | 17/11/2025 | 17/11/2025 | Cloud Journey - CI/CD |
| 3 | - **Giám sát với CloudWatch & X-Ray:**<br>+ Kích hoạt X-Ray tracing cho Lambda và API Gateway<br>+ Phân tích Service Map để tìm điểm nghẽn (bottleneck)<br>+ Xem Logs chi tiết trên CloudWatch Logs Insights | 18/11/2025 | 18/11/2025 | Cloud Journey - Monitoring |
| 4 | - **Giới thiệu AWS AppSync (GraphQL):**<br>+ Tìm hiểu sự khác biệt giữa REST API và GraphQL<br>+ Tạo AppSync API đơn giản kết nối với DynamoDB<br>+ Test query và mutation trên Console | 19/11/2025 | 19/11/2025 | Cloud Journey - AppSync |
| 5 | - **Thực hành nâng cao (Optional):**<br>+ Thử nghiệm AWS SAM (Serverless Application Model) để định nghĩa hạ tầng bằng code<br>+ Deploy ứng dụng bằng lệnh `sam deploy` | 20/11/2025 | 20/11/2025 | Cloud Journey - SAM |
| 6 | - **Tổng kết tuần 11:**<br>+ Review toàn bộ quá trình Hiện đại hóa ứng dụng<br>+ Chuẩn bị tư liệu và số liệu cho báo cáo cuối kỳ | 21/11/2025 | 21/11/2025 | Self-review |


### Kết quả đạt được tuần 11:

* Thiết lập được quy trình CI/CD tự động, giúp giảm thiểu lỗi con người khi deploy.
* Có khả năng debug và tối ưu hóa hiệu năng ứng dụng Serverless phức tạp nhờ X-Ray.
* Tiếp cận được công nghệ GraphQL mới mẻ thông qua AWS AppSync.
* Sẵn sàng cho việc tổng hợp và báo cáo kết quả thực tập.
