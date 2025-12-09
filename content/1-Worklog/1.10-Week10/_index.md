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
| 2 | - **Serverless Frontend:**<br>+ Build static website (HTML/JS) calling API Gateway<br>+ Host website on S3 with SSL (HTTPS)<br>+ Handle CORS on API Gateway<br><br>**SorcererXtreme Project:**<br>- **Frontend Integration:**<br>+ Connect Chat UI to Lambda Backend via API Gateway<br>+ Handle CORS and Authentication Token | 11/10/2025 | 11/10/2025 | [Cloud Journey - Serverless](https://cloudjourney.awsstudygroup.com/) |
| 3 | - **Authentication with Amazon Cognito:**<br>+ Create User Pool to manage users<br>+ Integrate Cognito into Frontend (Sign up/Sign in)<br>+ Protect API Gateway with Cognito Authorizer<br><br>**SorcererXtreme Project:**<br>- **UX Improvement:**<br>+ Add Loading Skeletons while waiting for response<br>+ Handle errors (Error Boundary) and Toast notifications | 11/11/2025 | 11/11/2025 | [Cloud Journey - Cognito](https://cloudjourney.awsstudygroup.com/) |
| 4 | - **Messaging & Eventing:**<br>+ Learn about Decoupling architecture<br>+ Create SQS Queue for pending orders<br>+ Create SNS Topic for email notifications<br><br>**SorcererXtreme Project:**<br>- **Cost Optimization:**<br>+ Setup AWS Budget for cost alerts<br>+ Review DynamoDB RCU/WCU (On-demand mode) | 11/12/2025 | 11/12/2025 | [Cloud Journey - SQS/SNS](https://cloudjourney.awsstudygroup.com/) |
| 5 | - **System Integration:**<br>+ Modify Lambda to push messages to SQS instead of processing immediately<br>+ Write Lambda Trigger to process messages from SQS<br>+ Send SNS notification upon completion<br><br>**SorcererXtreme Project:**<br>- **Performance Tuning:**<br>+ Optimize Lambda Cold Start (Provisioned Concurrency if needed)<br>+ Measure Lighthouse score and optimize Web Vitals | 11/13/2025 | 11/13/2025 | [Cloud Journey - Serverless](https://cloudjourney.awsstudygroup.com/) |
| 6 | - **Week 10 Review:**<br>+ Test full flow: Frontend -> API -> Lambda -> SQS -> Lambda -> DB -> SNS<br>+ Evaluate latency and load capacity | 11/14/2025 | 11/14/2025 | Self-review |


### Week 10 Achievements:

* Successfully built a complete Fullstack Serverless application.
* Learned professional API security and user management with Cognito.
* Understood and deployed Asynchronous architecture to prevent system bottlenecks.
* **SorcererXtreme Project:**
    * Fully connected Frontend and Backend, application runs smoothly.
    * Optimized User Experience (UX) and setup infrastructure cost controls.
