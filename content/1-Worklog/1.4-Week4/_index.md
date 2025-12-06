---
title: "Week 4 Worklog"
date: "2025-09-29"
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives:

* Deep dive into AWS VPC and networking concepts
* Understand S3 storage service and best practices
* Learn about RDS database services
* Practice hands-on labs with core AWS services

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| Monday (29/9) | - Review previous week's EC2 concepts <br> - Study AWS VPC fundamentals <br>&emsp; + Subnets and CIDR blocks <br>&emsp; + Route tables <br>&emsp; + Internet Gateway | 29/09/2025 | 29/09/2025 | <https://docs.aws.amazon.com/vpc/> |
| Tuesday (30/9) | - Continue VPC deep dive <br>&emsp; + Security Groups <br>&emsp; + Network ACLs <br>&emsp; + NAT Gateway <br> - Study VPC peering concepts | 30/09/2025 | 30/09/2025 | <https://cloudjourney.awsstudygroup.com/> |
| Wednesday (1/10) | - Introduction to Amazon S3 <br>&emsp; + Buckets and objects <br>&emsp; + Storage classes <br>&emsp; + Versioning <br> - S3 security and access control | 01/10/2025 | 01/10/2025 | <https://docs.aws.amazon.com/s3/> |
| Thursday (2/10) | - **Practice:** S3 hands-on lab <br>&emsp; + Create S3 bucket <br>&emsp; + Upload and manage objects <br>&emsp; + Configure bucket policies <br>&emsp; + Enable versioning | 02/10/2025 | 02/10/2025 | <https://cloudjourney.awsstudygroup.com/> |
| Friday (3/10) | - Study Amazon RDS basics <br>&emsp; + Database engines (MySQL, PostgreSQL) <br>&emsp; + Multi-AZ deployments <br>&emsp; + Read replicas <br> - RDS backup and restore | 03/10/2025 | 03/10/2025 | <https://docs.aws.amazon.com/rds/> |
| Monday (6/10) | **Office Workday** <br> - Comprehensive VPC hands-on lab <br>&emsp; + Create custom VPC with public/private subnets <br>&emsp; + Configure route tables and gateways <br>&emsp; + Set up security groups and NACLs <br> - Deploy EC2 instances in custom VPC <br> - Test connectivity between subnets | 06/10/2025 | 06/10/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Week 4 Achievements:

* Gained comprehensive understanding of AWS VPC architecture:
  * CIDR notation and IP addressing
  * Public vs private subnets
  * Route table configuration
  * Internet Gateway and NAT Gateway differences
  * VPC peering for inter-VPC communication

* Mastered VPC security components:
  * Security Groups (stateful firewall)
  * Network ACLs (stateless firewall)
  * Difference between Security Groups and NACLs
  * Best practices for network security

* Learned Amazon S3 storage service:
  * S3 bucket creation and management
  * Object storage concepts
  * Storage classes (Standard, IA, Glacier)
  * Versioning and lifecycle policies
  * Bucket policies and IAM permissions

* Completed hands-on S3 lab:
  * Created and configured S3 buckets
  * Uploaded objects and managed permissions
  * Implemented bucket policies for access control
  * Enabled versioning for data protection

![S3 Bucket Configuration](/images/week4/s3-bucket-setup.png)
*S3 bucket configuration with versioning enabled*

* Understood Amazon RDS fundamentals:
  * Managed database service benefits
  * Supported database engines
  * Multi-AZ for high availability
  * Read replicas for performance scaling
  * Automated backups and point-in-time recovery

* Successfully completed comprehensive VPC lab on office workday (6/10):
  * Created custom VPC with CIDR 10.0.0.0/16
  * Configured public subnet (10.0.1.0/24) and private subnet (10.0.2.0/24)
  * Set up Internet Gateway for public subnet
  * Configured NAT Gateway for private subnet internet access
  * Created and configured route tables
  * Deployed EC2 instances in both subnets
  * Tested connectivity and security group rules

![VPC Architecture](/images/week4/vpc-architecture.png)
*Custom VPC architecture with public and private subnets*

### Challenges Faced:

* Understanding the difference between Security Groups and Network ACLs took some time
* CIDR notation and subnet calculation required practice
* Configuring route tables correctly for NAT Gateway access

### Key Learnings:

* VPC is fundamental to AWS networking and security
* Proper subnet design is crucial for scalable architecture
* S3 is more than just storage - it's a platform for many AWS services
* RDS simplifies database management compared to self-managed databases

### Next Week Goals:

* Explore AWS Lambda and serverless computing
* Learn about CloudWatch for monitoring
* Start first blog translation
* Continue practicing with hands-on labs
