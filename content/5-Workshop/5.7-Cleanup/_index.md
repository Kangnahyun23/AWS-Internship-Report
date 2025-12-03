---
title: "Cleanup Resources"
weight: 7
chapter: false
pre: " <b> 5.7. </b> "
---

### Cleanup Checklist

To ensure no costs are incurred after completing the Workshop, delete resources in the following order:

1.  **Delete AWS WAF Web ACL:**
    *   Go to WAF Console -> Web ACLs -> Delete.
    *   *Note: Must Disassociate from CloudFront before deleting.*

2.  **Delete AWS Amplify App:**
    *   Go to Amplify Console -> Select App -> Actions -> Delete app.
    *   This automatically deletes: S3 Bucket (hosting), CloudFront Distribution (if default), Cognito User Pool, and DynamoDB Table (if any).

3.  **Delete Backend Resources (if manually created):**
    *   **RDS Database:** Go to RDS Console -> Databases -> Actions -> Delete. (Uncheck "Create final snapshot" if not needed).
    *   **Secrets Manager:** Schedule deletion for secret (minimum 7 days wait).
    *   **VPC:** Deleting VPC will automatically delete related Subnets, Internet Gateway, Route Tables. (Note: Must delete NAT Gateway and release Elastic IP first).

4.  **Check Billing Dashboard:**
    *   Go to Billing & Cost Management Dashboard to ensure no services are running in the background.

### Conclusion

Congratulations on successfully completing the **"Building Modern Serverless Frontend"** Workshop!

You have equipped yourself with comprehensive knowledge from Frontend (Next.js), DevOps (CI/CD), Security (WAF/Cognito) to Backend architecture (RDS/VPC). This is a solid foundation for you to join large-scale real-world projects.
