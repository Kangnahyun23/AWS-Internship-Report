---
title: "Event 5"
weight: 5
chapter: false
pre: " <b> 4.5. </b> "
---

### Workshop AWS Well-Architected Security Pillar

**Thời gian:** Thứ Bảy, ngày 29 tháng 11 năm 2025, 8:30 – 12:00

**Địa điểm:** Văn phòng AWS Vietnam

**Vai trò:** Người tham dự

### Mục Đích Của Sự Kiện
Workshop buổi sáng này cung cấp cái nhìn chuyên sâu toàn diện về AWS Well-Architected Security Pillar, bao gồm tất cả năm domain bảo mật: Identity & Access Management, Detection, Infrastructure Protection, Data Protection, và Incident Response. Phiên workshop được thiết kế để trang bị cho người tham dự kiến thức thực tế về việc triển khai các best practices bảo mật trong môi trường AWS.

### Agenda
**8:30 – 8:50 AM | Khai mạc & Nền tảng Security**
- Security Pillar trong Well-Architected Framework
- Nguyên tắc cốt lõi: Least Privilege – Zero Trust – Defense in Depth
- AWS Shared Responsibility Model

**8:50 – 9:30 AM | Pillar 1 — Identity & Access Management**
- Kiến trúc IAM hiện đại: Users, Roles, Policies
- IAM Identity Center: SSO, permission sets
- MFA, credential rotation, Access Analyzer

**9:30 – 9:55 AM | Pillar 2 — Detection**
- Detection & Continuous Monitoring: CloudTrail, GuardDuty, Security Hub
- Logging tại mọi tầng: VPC Flow Logs, ALB/S3 logs
- Detection-as-Code

**10:10 – 10:40 AM | Pillar 3 — Infrastructure Protection**
- Network & Workload Security: VPC segmentation, Security Groups vs NACLs
- WAF + Shield + Network Firewall

**10:40 – 11:10 AM | Pillar 4 — Data Protection**
- Encryption, Keys & Secrets: KMS, Encryption at-rest & in-transit
- Secrets Manager & Parameter Store

**11:10 – 11:40 AM | Pillar 5 — Incident Response**
- IR Playbook & Automation: IR lifecycle, Playbooks (Compromised IAM key, S3 public exposure)
- Auto-response với Lambda/Step Functions

**11:40 – 12:00 PM | Tổng kết & Q&A**

### Những Gì Tôi Học Được
- **Least Privilege là nền tảng:** Luôn bắt đầu với quyền tối thiểu và mở rộng khi cần.
- **Kiến trúc Zero Trust:** Không giả định tin cậy ngầm định, ngay cả trong mạng nội bộ.
- **Defense in Depth:** Yêu cầu kiểm soát bảo mật ở nhiều lớp.
- **Khả năng detection:** Phải được tự động hóa và liên tục.
- **Incident response playbooks:** Cần được tài liệu hóa và kiểm tra thường xuyên.

### Ứng Dụng Vào Công Việc
- Triển khai IAM Access Analyzer trong các dự án hiện tại.
- Thiết lập GuardDuty và Security Hub cho giám sát bảo mật tập trung.
- Tạo incident response playbooks cho các kịch bản phổ biến.
- Review và siết chặt Security Group rules theo nguyên tắc least privilege.
- Bật encryption cho tất cả data stores (S3, RDS, DynamoDB).

### Trải Nghiệm Cá Nhân
Bảo mật luôn là một chủ đề khô khan và khó nhằn đối với em, nhưng workshop này đã biến nó thành những kịch bản thực chiến rất hấp dẫn.
- Việc được hướng dẫn xử lý các tình huống như "lộ access key" hay "S3 bucket bị public" giúp em nhận ra những lỗi sơ đẳng này nguy hiểm đến mức nào.
- Em rất thích tư duy "Zero Trust" – không tin bất kỳ ai, kể cả trong mạng nội bộ. Nó thay đổi hoàn toàn cách em thiết kế kiến trúc hệ thống sau này.
- Các công cụ như GuardDuty hay Security Hub giống như những người bảo vệ thầm lặng, giúp em yên tâm hơn khi vận hành hệ thống trên Cloud.

### Bài Học Rút Ra
- **Security by Design:** Bảo mật không phải là thứ "cài thêm" sau khi làm xong sản phẩm, mà phải được tính toán ngay từ những dòng code đầu tiên.
- **Nguyên tắc Quyền tối thiểu (Least Privilege):** Dù việc cấu hình IAM role chi tiết rất tốn công, nhưng nó là chốt chặn quan trọng nhất để hạn chế thiệt hại khi có sự cố.
- **Luôn có kế hoạch ứng phó:** Sự cố có thể xảy ra bất cứ lúc nào. Việc chuẩn bị sẵn các Playbook (kịch bản ứng phó) giúp team không bị hoảng loạn và xử lý vấn đề một cách bài bản, nhanh chóng.
