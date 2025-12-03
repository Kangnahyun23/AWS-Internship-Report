---
title: "Week 10 Worklog"
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:

* Complete Serverless Application (Frontend + Backend).
* Secure application with Amazon Cognito.
* Asynchronous processing with SQS/SNS.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - **Serverless Frontend:**<br>+ Build static website (HTML/JS) calling API Gateway<br>+ Host website on S3 with SSL (HTTPS)<br>+ Handle CORS on API Gateway | 11/10/2025 | 11/10/2025 | Cloud Journey - Serverless |
| 3 | - **Authentication with Amazon Cognito:**<br>+ Create User Pool to manage users<br>+ Integrate Cognito into Frontend (Sign up/Sign in)<br>+ Protect API Gateway with Cognito Authorizer | 11/11/2025 | 11/11/2025 | Cloud Journey - Cognito |
| 4 | - **Messaging & Eventing:**<br>+ Learn about Decoupling architecture<br>+ Create SQS Queue for pending orders<br>+ Create SNS Topic for email notifications | 11/12/2025 | 11/12/2025 | Cloud Journey - SQS/SNS |
| 5 | - **System Integration:**<br>+ Modify Lambda to push messages to SQS instead of processing immediately<br>+ Write Lambda Trigger to process messages from SQS<br>+ Send SNS notification upon completion | 11/13/2025 | 11/13/2025 | Cloud Journey - Serverless |
| 6 | - **Week 10 Review:**<br>+ Test full flow: Frontend -> API -> Lambda -> SQS -> Lambda -> DB -> SNS<br>+ Evaluate latency and load capacity | 11/14/2025 | 11/14/2025 | Self-review |


### Week 10 Achievements:

* Successfully built a complete Fullstack Serverless application.
* Learned professional API security and user management with Cognito.
* Understood and deployed Asynchronous architecture to prevent system bottlenecks.
