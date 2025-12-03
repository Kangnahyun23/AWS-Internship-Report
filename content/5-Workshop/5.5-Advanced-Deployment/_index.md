---
title: "Optimization, Security & Monitoring"
weight: 5
chapter: false
pre: " <b> 5.5. </b> "
---

### 1. AWS WAF (Web Application Firewall)

Protects the application from common web exploits like SQL Injection, XSS, and DDoS.

![WAF Security Diagram](/images/waf_security_diagram_1764662992832.png)

**Rate Limiting Configuration:**
To prevent application-layer DDoS, set up a rate-based rule:
*   **Rule Type:** Rate-based rule.
*   **Rate Limit:** 100 requests / 5 minutes.
*   **Action:** Block.
*   **Scope:** Source IP address.

### 2. Amazon CloudFront (CDN)

*   **Caching:** Stores static files at Edge Locations.
*   **Invalidation:** Automatically invalidates old cache on new deploy.

### 3. Amazon Route 53 (Custom Domain)

Instead of using the long default Amplify domain (`...amplifyapp.com`), configure a professional custom domain.

1.  Purchase a domain on **Route 53**.
2.  In Amplify Console > **Domain management** > **Add domain**.
3.  Amplify automatically creates CNAME records and provisions SSL certificate.

### 4. Observability: CloudWatch & X-Ray

**Amazon CloudWatch (Logs & Metrics):**
Monitor metrics like CPU, Memory, Request count, and Error Rate.

**AWS X-Ray (Distributed Tracing):**
Visualize the entire journey of a Request: From Frontend -> API Gateway -> Lambda -> Database.

---

### My Experience

{{% notice tip %}}
**Saving CloudWatch Costs**
By default, CloudWatch Logs are stored **forever** (Never Expire). This will eat up your budget after a few months.
**Solution:** Always set **Retention Policy** to **1 week** or **1 month** for Dev/Staging environments. Only keep Production logs longer if Audit is required.
{{% /notice %}}

### Verification & Testing

**Test Case 1: Verify WAF (Rate Limiting)**
1.  Use a tool (like JMeter or Python script) to send 200 requests in 1 minute to the website.
2.  *Expected Result:* After the first ~100 requests, subsequent requests receive **403 Forbidden**.

**Test Case 2: Verify Domain & SSL**
1.  Access `https://your-domain.com`.
2.  Click the padlock icon in the address bar.
3.  *Expected Result:* "Connection is secure". Certificate issued by Amazon.
