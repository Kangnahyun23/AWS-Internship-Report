---
title: "Reference Backend Architecture (RDS & VPC)"
weight: 6
chapter: false
pre: " <b> 5.6. </b> "
---

### 1. VPC Architecture Model

The Backend is deployed within a **VPC (Virtual Private Cloud)** for maximum security:

![VPC Architecture Diagram](/images/vpc_rds_architecture_1764663010653.png)

*   **Public Subnet:** Contains **NAT Gateway** (for internal servers to access Internet) and **Bastion Host**.
*   **Private Subnet (App Layer):** Contains **AWS Lambda**.
*   **Private Subnet (Data Layer):** Contains **Amazon RDS (PostgreSQL)**.

### 2. Security Group Configuration (Firewall)

To ensure "Least Privilege" principle, we configure strict Security Group rules:

| Security Group | Inbound Rule | Outbound Rule | Description |
| :--- | :--- | :--- | :--- |
| **SG-Lambda** | None (or from API Gateway if needed) | Allow All to **SG-RDS** (Port 5432) | Lambda is only allowed to call Database. |
| **SG-RDS** | Allow TCP 5432 from **SG-Lambda** | None | Database only accepts connections from Lambda, denies all others. |

### 3. VPC Endpoints (PrivateLink)

To allow Lambda to access other AWS services (like S3, Secrets Manager, CloudWatch) without going through public Internet (via NAT Gateway), use **VPC Endpoints**.

---

### My Experience

{{% notice warning %}}
**Why not put Database in Public Subnet?**
Beginners often put RDS in Public Subnet for easy connection from local machine. **Never do this in Production!** Hackers can brute-force your password.
**Solution:** Always put RDS in Private Subnet. If you want to connect from local to debug, use a **Bastion Host** (Jump Server) or **AWS VPN Client**.
{{% /notice %}}

### Verification & Testing

**Test Case 1: Verify Lambda -> RDS Connection**
1.  Create a simple Lambda function executing query `SELECT NOW();`.
2.  Assign Lambda to Private Subnet and SG-Lambda.
3.  Run Test on AWS Console.
4.  *Expected Result:* Returns current time from Database.

**Test Case 2: Verify External Access Block**
1.  Try to connect directly to RDS Endpoint from local machine (via Internet).
2.  *Expected Result:* **Connection Timeout** (Cannot connect). This proves Database is securely protected inside VPC.
