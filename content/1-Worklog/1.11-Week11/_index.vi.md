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
| 2 | - **CI/CD với AWS CodePipeline:**<br>+ Tạo Repository trên AWS CodeCommit (hoặc GitHub)<br>+ Tạo Build Project với AWS CodeBuild (buildspec.yml)<br>+ Thiết lập Pipeline tự động deploy khi có code mới<br><br>**Dự án SorcererXtreme:**<br>- **Code Review:**<br>+ Review toàn bộ Codebase, Refactor components<br>+ Merge nhánh `develop` vào `main` | 17/11/2025 | 17/11/2025 | [Cloud Journey - CI/CD](https://cloudjourney.awsstudygroup.com/) |
| 3 | - **Giám sát với CloudWatch & X-Ray:**<br>+ Kích hoạt X-Ray tracing cho Lambda và API Gateway<br>+ Phân tích Service Map để tìm điểm nghẽn (bottleneck)<br>+ Xem Logs chi tiết trên CloudWatch Logs Insights<br><br>**Dự án SorcererXtreme:**<br>- **Production Deployment:**<br>+ Cấu hình Amplify Hosting (Production Branch)<br>+ Thiết lập biến môi trường (Environment Variables) | 18/11/2025 | 18/11/2025 | [Cloud Journey - Monitoring](https://cloudjourney.awsstudygroup.com/) |
| 4 | - **Giới thiệu AWS AppSync (GraphQL):**<br>+ Tìm hiểu sự khác biệt giữa REST API và GraphQL<br>+ Tạo AppSync API đơn giản kết nối với DynamoDB<br>+ Test query và mutation trên Console<br><br>**Dự án SorcererXtreme:**<br>- **Amplify Domain:**<br>+ Sử dụng domain mặc định của Amplify (`amplifyapp.com`)<br>+ Kiểm tra HTTPS/SSL mặc định | 19/11/2025 | 19/11/2025 | [Cloud Journey - AppSync](https://cloudjourney.awsstudygroup.com/) |
| 5 | - **Thực hành nâng cao (Optional):**<br>+ Thử nghiệm AWS SAM (Serverless Application Model) để định nghĩa hạ tầng bằng code<br>+ Deploy ứng dụng bằng lệnh `sam deploy`<br><br>**Dự án SorcererXtreme:**<br>- **Documentation:**<br>+ Viết README.md đầy đủ (Tech Stack, Setup)<br>+ Vẽ lại Architecture Diagram cập nhật | 20/11/2025 | 20/11/2025 | [Cloud Journey - SAM](https://cloudjourney.awsstudygroup.com/) |
| 6 | - **Tổng kết tuần 11:**<br>+ Review toàn bộ quá trình Hiện đại hóa ứng dụng<br>+ Chuẩn bị tư liệu và số liệu cho báo cáo cuối kỳ | 21/11/2025 | 21/11/2025 | Self-review |


### Kết quả đạt được tuần 11:

* Thiết lập được quy trình CI/CD tự động, giúp giảm thiểu lỗi con người khi deploy.
* Có khả năng debug và tối ưu hóa hiệu năng ứng dụng Serverless phức tạp nhờ X-Ray.
* Tiếp cận được công nghệ GraphQL mới mẻ thông qua AWS AppSync.
* Sẵn sàng cho việc tổng hợp và báo cáo kết quả thực tập.
* **Dự án SorcererXtreme:**
    * Deploy thành công ứng dụng ra môi trường Production với domain mặc định của Amplify.
    * Hoàn thiện tài liệu kỹ thuật, kiến trúc hệ thống và sẵn sàng demo.
