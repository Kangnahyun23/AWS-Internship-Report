---
title: "Week 5 Worklog"
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:

* Understand High Availability and Scalability.
* Configure EC2 Auto Scaling to automatically scale servers up/down.
* Comprehensive system monitoring with Amazon CloudWatch.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - **Prepare for Auto Scaling:**<br>+ Create AMI (Amazon Machine Image) from a configured EC2 Instance<br>+ Create Launch Template from that AMI | 10/06/2025 | 10/06/2025 | [Cloud Journey - Auto Scaling](https://cloudjourney.awsstudygroup.com/) |
| 3 | - **Configure Auto Scaling Group (ASG):**<br>+ Create ASG using Launch Template<br>+ Configure Min/Max/Desired capacity<br>+ Integrate with Application Load Balancer (ALB) | 10/07/2025 | 10/07/2025 | [Cloud Journey - Auto Scaling](https://cloudjourney.awsstudygroup.com/) |
| 4 | - **Amazon CloudWatch (Part 1):**<br>+ Learn about Metrics and Logs<br>+ View CPU, Network metrics of EC2 on CloudWatch Console | 10/08/2025 | 10/08/2025 | [Cloud Journey - CloudWatch](https://cloudjourney.awsstudygroup.com/) |
| 5 | - **Amazon CloudWatch (Part 2) & Scaling Policy:**<br>+ Create CloudWatch Alarm for CPU > 70%<br>+ Configure Dynamic Scaling Policy for ASG based on this Alarm<br>+ Perform Stress Test to trigger Auto Scaling | 10/09/2025 | 10/09/2025 | [Cloud Journey - CloudWatch](https://cloudjourney.awsstudygroup.com/) |
| 6 | - **Week 5 Review:**<br>+ Observe Scale-out and Scale-in processes<br>+ Create CloudWatch Dashboard to aggregate key metrics | 10/10/2025 | 10/10/2025 | Self-review |


### Week 5 Achievements:

* Built a system capable of self-healing and scaling according to actual demand.
* Understood the role of Load Balancer in traffic distribution.
* Proficiently used CloudWatch to monitor system "health".
* Successfully executed Stress Test scenario to verify Auto Scaling capabilities.
