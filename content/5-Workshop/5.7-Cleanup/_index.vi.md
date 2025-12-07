---
title: "Dọn dẹp tài nguyên"
weight: 7
chapter: false
pre: " <b> 5.7. </b> "
---

# Quy trình dọn dẹp (Cleanup Checklist)

Sau khi hoàn thành Workshop, việc dọn dẹp là **bắt buộc** để tránh phát sinh chi phí "oan" từ AWS. Vì chúng ta sử dụng Services Serverless (Amplify, Lambda, Bedrock), việc dọn dẹp khá đơn giản nhưng cần kỹ lưỡng.

### 1. Xóa ứng dụng trên AWS Amplify

Đây là bước quan trọng nhất. Xóa App trên Amplify sẽ tự động dọn dẹp 80% tài nguyên liên quan (Hosting S3, CloudFront, CI/CD Pipeline).

1.  Truy cập **AWS Amplify Console**.
2.  Chọn ứng dụng **SorcererXtreme**.
3.  Vào tab **Actions** (góc trên bên phải) -> Chọn **Delete app**.
4.  Nhập cụm từ xác nhận (thường là `delete`) và nhấn Confirm.

### 2. Dọn dẹp Database & External Services

Vì **NeonDB** và **Pinecone** là dịch vụ bên thứ 3 (không nằm trong gói Amplify Delete), bạn cần xóa thủ công:

*   **NeonDB:**
    *   Đăng nhập Console Neon.
    *   Vào **Settings** của Project -> **Delete Project**.
*   **Pinecone:**
    *   Đăng nhập Console Pinecone.
    *   Xóa **Index** (ví dụ `tarot-knowledge-base`) để dừng tính phí lưu trữ vector.

### 3. Dọn dẹp tài nguyên AWS thủ công (Nếu có tạo lẻ)

Nếu trong quá trình làm bạn có tạo thêm tài nguyên ngoài Amplify, hãy kiểm tra:

*   **Amazon Bedrock:** Bedrock tính tiền theo Request (On-demand) nên không cần xóa "Model". Tuy nhiên nếu bạn có tạo **Knowledge Base** riêng, hãy xóa nó.
*   **Amazon Cognito:** Kiểm tra xem User Pool đã mất chưa (thường Amplify xóa giúp rồi).
*   **Parameter Store:** Vào AWS Systems Manager > Parameter Store > Xóa các key như `/sorcerer/neon_db_url`, `/sorcerer/pinecone_api_key`.

### 4. Kiểm tra lần cuối (Billing Dashboard)

Để chắc chắn 100%:
1.  Truy cập **AWS Billing Dashboard**.
2.  Kiểm tra mục **"Bills"**.
3.  Đợi 24h để hệ thống cập nhật và đảm bảo không có chi phí mới phát sinh từ các dịch vụ lạ.

---

### Lời kết

Chúc mừng bạn đã đi đến cuối hành trình! 🎉

Bạn đã hoàn thành việc xây dựng **SorcererXtreme** - một ứng dụng kết hợp giữa nghệ thuật Frontend (Next.js), sức mạnh Cloud (AWS Amplify) và trí tuệ nhân tạo (Bedrock RAG).

Hy vọng kiến thức từ Workshop này sẽ giúp bạn tự tin hơn khi apply vào các vị trí **Cloud-Native Frontend Developer** hoặc **Fullstack Developer**.

Hẹn gặp lại bạn ở các Workshop nâng cao! 👋
