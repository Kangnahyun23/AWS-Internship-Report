---
title: "Workshop"
weight: 5
chapter: false
pre: " <b> 5. </b> "
---

# Building Serverless Frontend with Next.js & AWS Amplify

### Workshop Overview

Welcome to the **Building Modern Serverless Frontend** Workshop. This is not just a coding tutorial, but a journey distilled from real-world experience to build a **Production-Ready** web application.

We will solve the problem: *How to create an AI application with a beautiful interface, fast speed, and high security without managing servers?*

**Target Audience:**
*   Frontend Developers wanting to learn Cloud & DevOps.
*   Students wanting a "cool" project with the latest tech.
*   Anyone who loves Next.js and AWS.

### System Architecture

Instead of just running code locally, we will build a complete system on AWS:

![Architecture Diagram](/images/workshop_architecture_diagram_1764662750000.png)

**Data Flow:**
1.  **User** accesses website via custom domain (Route 53).
2.  Request passes through **AWS WAF** to filter malicious traffic.
3.  **CloudFront (CDN)** returns static content (HTML/CSS/JS) instantly from Edge Location.
4.  When User chats with AI, Request is sent to **API Gateway**.
5.  **Cognito** authenticates User (ensuring only logged-in users can chat).
6.  **Lambda** processes logic and calls **RDS Database** to save history.

### AWS Services Used

| Category | Service |
| :--- | :--- |
| **Compute** | AWS Lambda |
| **Frontend & Hosting** | AWS Amplify Hosting |
| **Authentication** | Amazon Cognito |
| **API** | Amazon API Gateway |
| **Database** | Amazon RDS (PostgreSQL) |
| **Security** | AWS WAF |
| **CDN & DNS** | Amazon CloudFront, Amazon Route 53 |
| **Monitoring** | Amazon CloudWatch, AWS X-Ray |

### Estimated Time & Cost

| Item | Details |
| :--- | :--- |
| **Time** | 2-3 hours |
| **Level** | Intermediate |
| **Cost** | ~$5-10 (If cleaned up after workshop) |

### Workshop Content

The workshop is divided into 7 parts, from basic to advanced:

1.  [**Preparation:**](5.1-preparation/) Setting up VS Code like a Senior Dev.
2.  [**UI Implementation:**](5.2-ui-implementation/) Coding "Mystical" interface with TailwindCSS.
3.  [**Integration:**](5.3-integration/) Connecting secure APIs with Custom Hooks.
4.  [**CI/CD Pipeline:**](5.4-deployment/) Automated deployment, no more manual file copying.
5.  [**Advanced Deployment:**](5.5-advanced-deployment/) Optimizing performance and security (WAF, CDN).
6.  [**Backend Architecture:**](5.6-backend-architecture/) Understanding the backend system (VPC, RDS).
7.  [**Cleanup:**](5.7-cleanup/) Cleaning up to avoid unexpected costs.

---
{{% notice tip %}}
**Advice:** Don't just copy-paste code. Read the **"My Experience"** section at the end of each article carefully to avoid the mistakes I spent hours debugging!
{{% /notice %}}