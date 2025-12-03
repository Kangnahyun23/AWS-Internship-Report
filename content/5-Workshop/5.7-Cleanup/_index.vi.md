---
title: "Dọn dẹp tài nguyên"
weight: 7
chapter: false
pre: " <b> 5.7. </b> "
---

### Quy trình dọn dẹp (Cleanup Checklist)

Để đảm bảo không phát sinh chi phí sau khi hoàn thành Workshop, hãy thực hiện xóa tài nguyên theo thứ tự sau:

1.  **Xóa AWS WAF Web ACL:**
    *   Vào WAF Console -> Web ACLs -> Delete.
    *   *Lưu ý: Phải Disassociate khỏi CloudFront trước khi xóa.*

2.  **Xóa ứng dụng AWS Amplify:**
    *   Vào Amplify Console -> Chọn App -> Actions -> Delete app.
    *   Việc này sẽ tự động xóa: S3 Bucket (hosting), CloudFront Distribution (nếu mặc định), Cognito User Pool, và DynamoDB Table (nếu có).

3.  **Xóa tài nguyên Backend (nếu tạo thủ công):**
    *   **RDS Database:** Vào RDS Console -> Databases -> Actions -> Delete. (Bỏ chọn "Create final snapshot" nếu không cần thiết).
    *   **Secrets Manager:** Schedule deletion cho secret (thời gian chờ tối thiểu 7 ngày).
    *   **VPC:** Xóa VPC sẽ tự động xóa các Subnet, Internet Gateway, Route Table liên quan. (Lưu ý: Phải xóa NAT Gateway và giải phóng Elastic IP trước).

4.  **Kiểm tra Billing Dashboard:**
    *   Vào Billing & Cost Management Dashboard để đảm bảo không còn dịch vụ nào đang chạy ngầm.

### Lời kết

Chúc mừng bạn đã hoàn thành xuất sắc Workshop **"Xây dựng Frontend Serverless hiện đại"**!

Bạn đã trang bị cho mình những kiến thức toàn diện từ Frontend (Next.js), DevOps (CI/CD), Security (WAF/Cognito) đến kiến trúc Backend (RDS/VPC). Đây là hành trang vững chắc để bạn tham gia vào các dự án thực tế quy mô lớn.
