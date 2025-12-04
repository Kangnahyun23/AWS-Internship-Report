---
title: "Event 5"
weight: 5
chapter: false
pre: " <b> 4.5. </b> "
---

### AWS Well-Architected Security Pillar Workshop

**Time:** Saturday, November 29, 2025, 8:30 – 12:00

**Location:** AWS Vietnam Office

**Role:** Attendee

### Event Purpose
This morning workshop provided a comprehensive deep dive into the AWS Well-Architected Security Pillar, covering all five security domains: Identity & Access Management, Detection, Infrastructure Protection, Data Protection, and Incident Response. The session was designed to equip attendees with practical knowledge on implementing security best practices in AWS environments.

### Agenda
**8:30 – 8:50 AM | Opening & Security Foundations**
- Security Pillar in Well-Architected Framework
- Core Principles: Least Privilege – Zero Trust – Defense in Depth
- AWS Shared Responsibility Model

**8:50 – 9:30 AM | Pillar 1 — Identity & Access Management**
- Modern IAM Architecture: Users, Roles, Policies
- IAM Identity Center: SSO, permission sets
- MFA, credential rotation, Access Analyzer

**9:30 – 9:55 AM | Pillar 2 — Detection**
- Detection & Continuous Monitoring: CloudTrail, GuardDuty, Security Hub
- Logging at all layers: VPC Flow Logs, ALB/S3 logs
- Detection-as-Code

**10:10 – 10:40 AM | Pillar 3 — Infrastructure Protection**
- Network & Workload Security: VPC segmentation, Security Groups vs NACLs
- WAF + Shield + Network Firewall

**10:40 – 11:10 AM | Pillar 4 — Data Protection**
- Encryption, Keys & Secrets: KMS, Encryption at-rest & in-transit
- Secrets Manager & Parameter Store

**11:10 – 11:40 AM | Pillar 5 — Incident Response**
- IR Playbook & Automation: IR lifecycle, Playbooks (Compromised IAM key, S3 public exposure)
- Auto-response with Lambda/Step Functions

**11:40 – 12:00 PM | Wrap-up & Q&A**

### What I Learned
- **Least Privilege is foundational:** Always start with minimum permissions and expand as needed.
- **Zero Trust Architecture:** Do not assume implicit trust, even within internal networks.
- **Defense in Depth:** Requires security controls at multiple layers.
- **Detection capabilities:** Must be automated and continuous.
- **Incident response playbooks:** Need to be documented and tested regularly.

### Application to Work
- Deploy IAM Access Analyzer in current projects.
- Set up GuardDuty and Security Hub for centralized security monitoring.
- Create incident response playbooks for common scenarios.
- Review and tighten Security Group rules based on least privilege.
- Enable encryption for all data stores (S3, RDS, DynamoDB).

### Personal Experience
Security has always been a dry and difficult topic for me, but this workshop turned it into engaging combat scenarios.
- Being guided through handling situations like "exposed access keys" or "public S3 buckets" made me realize how dangerous these basic errors can be.
- I really like the "Zero Trust" mindset – trust no one, even within the internal network. It completely changes how I design system architectures from now on.
- Tools like GuardDuty or Security Hub act like silent guardians, giving me peace of mind when operating systems on the Cloud.

### Key Takeaways
- **Security by Design:** Security is not an "add-on" after the product is finished, but must be calculated from the very first lines of code.
- **Least Privilege Principle:** Although configuring detailed IAM roles is time-consuming, it is the most important checkpoint to limit damage when incidents occur.
- **Always have a Response Plan:** Incidents can happen at any time. Having Playbooks ready helps the team avoid panic and handle issues systematically and quickly.
