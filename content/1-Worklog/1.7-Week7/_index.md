---
title: "Week 7 Worklog"
date: 2025-10-24
draft: false
weight: 7
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives
*   Enhance knowledge of AWS Networking (Networking Advanced).
*   Optimize content delivery with CDN (CloudFront).
*   Secure web applications at the edge (Edge Security).

### Tasks for this week

| Day | Task | Start Date | End Date | Resources |
| :--- | :--- | :--- | :--- | :--- |
| Mon | **Networking Workshop (Part 1):**<br>- Learn about VPC Peering (connecting 2 VPCs)<br>- Practice creating 2 VPCs and setting up Peering Connection<br>- Configure Route Tables for VPC communication<br><br>**SorcererXtreme Project:**<br>- **UI Design:**<br>+ Build Global Layout & Sidebar (Glassmorphism)<br>+ Responsive Design for Mobile/Tablet | 10/20/2025 | 10/20/2025 | [Cloud Journey - Networking](https://cloudjourney.awsstudygroup.com/) |
| Tue | **Networking Workshop (Part 2):**<br>- Learn about Site-to-Site VPN (theory)<br>- Practice simulating VPN connection (if possible) or learn about Transit Gateway<br>- VPC Endpoints (PrivateLink) for accessing internal AWS services<br><br>**SorcererXtreme Project:**<br>- **Frontend Dev:**<br>+ Build `ChatComponent`: Message bubbles, Input<br>+ Add Animations (Framer Motion) | 21/10/2025 | 21/10/2025 | [Cloud Journey - Networking](https://cloudjourney.awsstudygroup.com/) |
| Wed | **Amazon CloudFront (Part 1):**<br>- Learn about CDN and Edge Locations<br>- Create CloudFront Distribution for S3 Bucket (done in Week 3)<br>- Configure OAI (Origin Access Identity) to secure S3<br><br>**SorcererXtreme Project:**<br>- **Cognito Backend:**<br>+ Configure `amplify/auth.ts`<br>+ Define Email/Password login | 10/22/2025 | 10/22/2025 | [Cloud Journey - CloudFront](https://cloudjourney.awsstudygroup.com/) |
| Thu | **Amazon CloudFront (Part 2) & WAF:**<br>- Configure Custom Domain and SSL Certificate (ACM) for CloudFront<br>- Learn about AWS WAF (Web Application Firewall)<br>- Create simple WAF ACL to block IPs or Geo-blocking attached to CloudFront<br><br>**Midterm Revision (Part 1):**<br>- Secure Architectures (IAM, MFA, SCP, Encryption, Security Groups, WAF...)<br>- Resilient Architectures (Multi-AZ, Auto Scaling, Route 53...)<br><br>**SorcererXtreme Project:**<br>- **Auth Frontend:**<br>+ Create Login/Register pages with Amplify UI<br>+ Customize Form Theme | 10/23/2025 | 10/23/2025 | [Cloud Journey - CloudFront](https://cloudjourney.awsstudygroup.com/)<br>Midterm Revision |
| Fri | **Week 7 Review & Revision:**<br>- Check website access speed via CDN vs direct S3<br>- Review all Networking and Content Delivery knowledge<br><br>**Midterm Revision (Part 2):**<br>- High-Performing Architectures (EC2 Auto Scaling, Lambda, S3, Caching...)<br>- Cost-Optimized Architectures (Cost Explorer, Savings Plans, Storage Tiering...) | 24/10/2025 | 24/10/2025 | Self-review<br>Midterm Revision |

### Week 7 Outcomes
*   Deep understanding of network architecture in AWS, how to connect VPCs.
*   Successfully deployed CDN to speed up page loading for global users.
*   Know how to secure origin content (S3) from direct access.
*   Understood how to protect applications from basic web attacks with WAF.
* **SorcererXtreme Project:**
    * Completed Chat UI with Mystical/Glassmorphism style.
    * Successfully integrated user authentication (Auth) with Amazon Cognito.
