---
title: "Worklog Tuần 4"
date: "2025-09-29"
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:

* Tìm hiểu sâu về AWS VPC và các khái niệm networking
* Hiểu về dịch vụ lưu trữ S3 và best practices
* Học về dịch vụ cơ sở dữ liệu RDS
* Thực hành hands-on labs với các dịch vụ AWS cốt lõi

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| Thứ Hai (29/9) | - Ôn tập các khái niệm EC2 tuần trước <br> - Học AWS VPC cơ bản <br>&emsp; + Subnets và CIDR blocks <br>&emsp; + Route tables <br>&emsp; + Internet Gateway | 29/09/2025 | 29/09/2025 | <https://docs.aws.amazon.com/vpc/> |
| Thứ Ba (30/9) | - Tiếp tục tìm hiểu sâu VPC <br>&emsp; + Security Groups <br>&emsp; + Network ACLs <br>&emsp; + NAT Gateway <br> - Học về VPC peering | 30/09/2025 | 30/09/2025 | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Tư (1/10) | - Giới thiệu Amazon S3 <br>&emsp; + Buckets và objects <br>&emsp; + Storage classes <br>&emsp; + Versioning <br> - Bảo mật và kiểm soát truy cập S3 | 01/10/2025 | 01/10/2025 | <https://docs.aws.amazon.com/s3/> |
| Thứ Năm (2/10) | - **Thực hành:** S3 hands-on lab <br>&emsp; + Tạo S3 bucket <br>&emsp; + Upload và quản lý objects <br>&emsp; + Cấu hình bucket policies <br>&emsp; + Bật versioning | 02/10/2025 | 02/10/2025 | <https://cloudjourney.awsstudygroup.com/> |
| Thứ Sáu (3/10) | - Học Amazon RDS cơ bản <br>&emsp; + Database engines (MySQL, PostgreSQL) <br>&emsp; + Multi-AZ deployments <br>&emsp; + Read replicas <br> - RDS backup và restore | 03/10/2025 | 03/10/2025 | <https://docs.aws.amazon.com/rds/> |
| Thứ Hai (6/10) | **Ngày làm việc tại văn phòng** <br> - VPC hands-on lab toàn diện <br>&emsp; + Tạo custom VPC với public/private subnets <br>&emsp; + Cấu hình route tables và gateways <br>&emsp; + Thiết lập security groups và NACLs <br> - Deploy EC2 instances trong custom VPC <br> - Test kết nối giữa các subnets | 06/10/2025 | 06/10/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 4:

* Hiểu toàn diện về kiến trúc AWS VPC:
  * CIDR notation và IP addressing
  * Public vs private subnets
  * Cấu hình route table
  * Sự khác biệt giữa Internet Gateway và NAT Gateway
  * VPC peering cho kết nối giữa các VPC

* Nắm vững các thành phần bảo mật VPC:
  * Security Groups (stateful firewall)
  * Network ACLs (stateless firewall)
  * Sự khác biệt giữa Security Groups và NACLs
  * Best practices cho network security

* Học được dịch vụ lưu trữ Amazon S3:
  * Tạo và quản lý S3 bucket
  * Khái niệm object storage
  * Storage classes (Standard, IA, Glacier)
  * Versioning và lifecycle policies
  * Bucket policies và IAM permissions

* Hoàn thành S3 hands-on lab:
  * Tạo và cấu hình S3 buckets
  * Upload objects và quản lý permissions
  * Triển khai bucket policies để kiểm soát truy cập
  * Bật versioning để bảo vệ dữ liệu

![Cấu hình S3 Bucket](/images/week4/s3-bucket-setup.png)
*Cấu hình S3 bucket với versioning được bật*

* Hiểu về Amazon RDS cơ bản:
  * Lợi ích của managed database service
  * Các database engines được hỗ trợ
  * Multi-AZ cho high availability
  * Read replicas cho performance scaling
  * Automated backups và point-in-time recovery

* Hoàn thành thành công VPC lab toàn diện vào ngày làm việc (6/10):
  * Tạo custom VPC với CIDR 10.0.0.0/16
  * Cấu hình public subnet (10.0.1.0/24) và private subnet (10.0.2.0/24)
  * Thiết lập Internet Gateway cho public subnet
  * Cấu hình NAT Gateway cho private subnet truy cập internet
  * Tạo và cấu hình route tables
  * Deploy EC2 instances trong cả hai subnets
  * Test kết nối và security group rules

![Kiến trúc VPC](/images/week4/vpc-architecture.png)
*Kiến trúc custom VPC với public và private subnets*

### Thách thức gặp phải:

* Hiểu sự khác biệt giữa Security Groups và Network ACLs mất một chút thời gian
* CIDR notation và tính toán subnet cần thực hành
* Cấu hình route tables đúng cho NAT Gateway access

### Bài học quan trọng:

* VPC là nền tảng cho AWS networking và security
* Thiết kế subnet đúng cách rất quan trọng cho kiến trúc có thể mở rộng
* S3 không chỉ là storage - nó là nền tảng cho nhiều dịch vụ AWS
* RDS đơn giản hóa quản lý database so với self-managed databases

### Mục tiêu tuần tới:

* Khám phá AWS Lambda và serverless computing
* Học về CloudWatch cho monitoring
* Bắt đầu dịch blog đầu tiên
* Tiếp tục thực hành với hands-on labs


