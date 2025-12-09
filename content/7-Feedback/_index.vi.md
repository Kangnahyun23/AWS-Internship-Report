---
title: "Chia sẻ, đóng góp ý kiến"
weight: 7
chapter: false
pre: " <b> 7. </b> "
---

### 1. Chia sẻ kiến thức (Technical Sharings)

Sau quá trình thực hiện dự án **SorcererXtreme** từ con số 0 đến khi deploy lên AWS, mình rút ra được 3 bài học tâm đắc nhất mà mình tin là sẽ hữu ích cho bất kỳ Frontend Developer nào muốn lấn sân sang Cloud:

#### A. Amplify Gen 2: "Cứu cánh" cho Frontend Dev
Trước đây, mình luôn nghĩ việc dựng Backend (Auth, API, Database) là một cơn ác mộng vì phải học quá nhiều thứ (EC2, VPC, Nginx...). Nhưng với **AWS Amplify Gen 2**, mọi thứ thay đổi hoàn toàn:
*   **Code-First:** Mình chỉ cần viết TypeScript (`amplify/auth.ts`, `amplify/data.ts`), không cần click chuột cấu hình thủ công.
*   **Fullstack Type Safety:** Kiểu dữ liệu từ Backend được map tự động sang Frontend, giúp code không bao giờ bị lỗi sai tên biến.
*   **Kết luận:** Serverless đã hạ thấp rào cản gia nhập Cloud xuống mức tối thiểu.

#### B. AI không phải là phép thuật (Understanding AI Integration)
Mình từng nghĩ tích hợp AI vào web rất phức tạp. Nhưng thực tế với **Amazon Bedrock**, nó chỉ đơn giản là... gọi API.
*   **Mô hình RAG (Retrieval-Augmented Generation):** Mình học được cách làm cho AI "thông minh" hơn bằng cách cung cấp dữ liệu riêng (Sách Tarot, Kiến thức Chiêm tinh) lưu trong Pincone Vector DB.
*   **Bài học:** Đừng chỉ dùng AI, hãy "dạy" AI bằng dữ liệu của bạn.

#### C. Tư duy "Serverless First"
Chuyển từ tư duy "Thuê Server" sang "Serverless" giúp mình tối ưu được rất nhiều:
*   **Chi phí:** Không ai dùng web thì không mất tiền (Lambda chỉ tính tiền khi chạy).
*   **Vận hành:** Không lo server sập khi có nhiều người vào cùng lúc (Amplify tự động scale).

---

### 2. Đánh giá chung (General Evaluation)

Dưới đây là những cảm nhận của mình về môi trường thực tập tại **AWS First Cloud Journey**:

**1. Môi trường làm việc**

Môi trường làm việc rất chuyên nghiệp nhưng cũng đầy cởi mở. Các thành viên trong team luôn sẵn sàng hỗ trợ nhau (Google Meet/Discord) bất kể ngày đêm. Không gian làm việc từ xa (Remote) nhưng quy trình quản lý bằng GitHub rất chặt chẽ, giúp mình không bị "lạc trôi".

**2. Sự hỗ trợ của mentor / team admin**

Mentor hướng dẫn rất chi tiết, giải thích rõ ràng khi mình chưa hiểu và luôn khuyến khích mình đặt câu hỏi. Team admin hỗ trợ các thủ tục, tài liệu và tạo điều kiện để mình làm việc thuận lợi. Mình đánh giá cao việc mentor cho phép mình thử và tự xử lý vấn đề thay vì chỉ đưa đáp án.

**3. Sự phù hợp công việc**

Dự án **SorcererXtreme** thực sự là một "bài test" hoàn hảo. Nó vừa đủ khó (Next.js 14, AI, Vector DB) để thách thức kiến thức cũ, nhưng cũng đủ thú vị để tạo cảm hứng mỗi ngày.

**4. Cơ hội phát triển kỹ năng**

Ngoài kỹ thuật (Next.js, AWS), mình học được rất nhiều về **Soft Skills**: Cách viết báo cáo (Documentation), cách trình bày vấn đề (Communication) và quản lý thời gian (Time Management) để kịp deadline hàng tuần.

**5. Văn hóa & Tinh thần đồng đội**

"Work hard, Play hard". Dù áp lực về tiến độ dự án (đặc biệt là giai đoạn tích hợp AI), nhưng không khí trong team luôn tích cực. Mọi người coi bug là "tính năng" để cùng nhau tìm cách fix, thay vì đổ lỗi.

---

### 3. Một số câu hỏi khác

*   **Điều bạn hài lòng nhất trong thời gian thực tập?**
    Điều mình tâm đắc nhất là được tiếp cận công nghệ mới nhất (**Amplify Gen 2**). Thay vì học lý thuyết suông, mình được "thực chiến" xây dựng dự án **SorcererXtreme** từ A-Z. Cảm giác nhìn thấy sản phẩm của mình chạy mượt mà trên môi trường Production và tích hợp thành công AI là vô cùng thỏa mãn.

*   **Điều bạn nghĩ công ty cần cải thiện cho các thực tập sinh sau?**
    Mình nghĩ chương trình nên bổ sung thêm một buổi **Workshop chuyên sâu về Cost Optimization** (Tối ưu chi phí) ngay từ tuần đầu. Với các dịch vụ Cloud, chỉ cần quên tắt một Resource (như NAT Gateway hay RDS) là có thể phát sinh chi phí lớn, điều này đôi khi gây lo lắng cho các bạn mới.

*   **Nếu giới thiệu cho bạn bè, bạn có khuyên họ thực tập ở đây không? Vì sao?**
    Chắc chắn là **CÓ**. Đây không phải là nơi để "pha trà rót nước". Bạn sẽ bị "ném" vào dự án thật, phải tự bơi (với phao cứu sinh là Mentor) và áp lực deadline thật. Đó là cách trưởng thành nhanh nhất cho một sinh viên IT.

### 4. Đề xuất & mong muốn

*   **Bạn có đề xuất gì để cải thiện trải nghiệm trong kỳ thực tập?**
    Nên có thêm các buổi **Tech Talk** ngắn hàng tuần để các thực tập sinh chia sẻ về công nghệ mình đang tìm hiểu (ví dụ: tuần này mình tìm hiểu về Vector DB, tuần sau bạn khác chia sẻ về DevOps). Điều này giúp lan tỏa kiến thức chéo giữa các team.

*   **Bạn có muốn tiếp tục chương trình này trong tương lai?**
    Mình rất mong muốn được tiếp tục đồng hành cùng **AWS First Cloud Journey** ở các giai đoạn nâng cao hơn (Advanced Level), hoặc có cơ hội tham gia vào các dự án thực tế lớn hơn của công ty để rèn luyện kỹ năng Solution Architect.

*   **Góp ý khác (tự do chia sẻ):**
    Cảm ơn Team Admin và Mentor đã luôn support nhiệt tình. Một hành trình gần 4 tháng không quá dài nhưng đủ để thay đổi tư duy lập trình của mình từ "Coder" sang "Builder".