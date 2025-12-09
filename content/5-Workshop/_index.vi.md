---
title: "Workshop"
date: "2025-12-09"
weight: 5
chapter: false
pre: " <b> 5. </b> "
---

# InsightHR - Workshop Nền tảng Tự động hóa HR Serverless

## Tổng quan

**InsightHR** là một nền tảng tự động hóa HR hiện đại, hoàn toàn serverless được xây dựng trên AWS, minh họa các phương pháp tốt nhất cho phát triển ứng dụng cloud-native. Workshop này hướng dẫn bạn xây dựng và triển khai một ứng dụng hoàn chỉnh sẵn sàng cho production sử dụng các dịch vụ AWS.

## Những gì bạn sẽ xây dựng

Một hệ thống quản lý HR toàn diện bao gồm:

- **Quản lý Nhân viên**: Các thao tác CRUD đầy đủ với bộ lọc nâng cao
- **Theo dõi Hiệu suất**: Điểm hiệu suất theo quý và quản lý KPI
- **Hệ thống Chấm công**: Check-in/check-out thời gian thực với lịch sử theo dõi
- **AI Chatbot**: Truy vấn ngôn ngữ tự nhiên được hỗ trợ bởi AWS Bedrock (Claude 3)
- **Dashboard Phân tích**: Trực quan hóa hiệu suất tương tác
- **Kiểm soát Truy cập Dựa trên Vai trò**: Vai trò Admin, Manager và Employee
- **Xác thực**: Email/password và Google OAuth qua AWS Cognito

## Điểm nổi bật Kiến trúc

- ✅ **100% Serverless** - Không có EC2 instances cần quản lý
- ✅ **Có khả năng mở rộng** - Tự động scale theo nhu cầu
- ✅ **Tiết kiệm Chi phí** - Chỉ trả tiền cho những gì bạn sử dụng
- ✅ **Bảo mật** - Bảo mật tích hợp với Cognito và IAM
- ✅ **Stack Hiện đại** - React + TypeScript + Python
- ✅ **Sẵn sàng Production** - Giám sát CloudWatch và custom domain

## Các dịch vụ AWS được sử dụng

- **Frontend**: S3 + CloudFront + Route53
- **Backend**: Lambda + API Gateway + DynamoDB
- **Authentication**: Cognito User Pools
- **AI/ML**: Amazon Bedrock (Claude 3 Haiku)
- **Monitoring**: CloudWatch + Synthetics Canaries
- **Security**: IAM + ACM (SSL Certificates)

## Nội dung Workshop

1. [Tổng quan Workshop](5.1-workshop-overview)
2. [Yêu cầu tiên quyết](5.2-prerequisite/)
3. [Kiến trúc Dự án](5.3-architecture/)
4. [Thiết lập Môi trường AWS](5.4-setup-aws/)
5. [Thiết lập Database (DynamoDB)](5.5-database-setup/)
6. [Dịch vụ Xác thực](5.6-authentication/)
7. [Dịch vụ Backend](5.7-backend-services/)
8. [Phát triển Frontend](5.8-frontend/)
9. [Triển khai](5.9-deployment/)
10. [Kiểm thử & Giám sát](5.10-testing/)
11. [Dọn dẹp](5.11-cleanup/)

## Kết quả Học tập

Sau khi hoàn thành workshop này, bạn sẽ học được:

- Cách thiết kế và triển khai kiến trúc serverless
- Các phương pháp tốt nhất cho AWS Lambda và API Gateway
- Mô hình hóa và tối ưu hóa dữ liệu DynamoDB
- Luồng xác thực AWS Cognito
- Tích hợp với AWS Bedrock cho khả năng AI
- Cấu hình CloudFront CDN
- Nguyên tắc Infrastructure as Code
- Chiến lược triển khai production
- Kỹ thuật tối ưu hóa chi phí

## Yêu cầu tiên quyết

- Tài khoản AWS với quyền phù hợp
- Kiến thức cơ bản về JavaScript/TypeScript và Python
- Quen thuộc với React framework
- Hiểu biết về REST APIs
- AWS CLI đã được cài đặt và cấu hình

## Thời gian Ước tính

- **Workshop Đầy đủ**: 4-6 giờ
- **Chỉ Tính năng Cốt lõi**: 2-3 giờ

## Ước tính Chi phí

Chạy workshop này sẽ phát sinh chi phí AWS tối thiểu:

- **DynamoDB**: ~$0.50/tháng (on-demand pricing)
- **Lambda**: Free tier bao phủ hầu hết việc sử dụng
- **S3 + CloudFront**: ~$1-2/tháng
- **API Gateway**: ~$0.10/tháng
- **Bedrock**: ~$0.0004 mỗi truy vấn
- **Tổng cộng**: ~$2-5/tháng cho development

{{% notice tip %}}
Nhớ dọn dẹp tài nguyên sau khi hoàn thành workshop để tránh phí tiếp tục.
{{% /notice %}}

## Hỗ trợ

Đối với câu hỏi hoặc vấn đề trong workshop:

- Kiểm tra các phần khắc phục sự cố trong mỗi module
- Xem lại các liên kết tài liệu AWS được cung cấp
- Tham khảo GitHub repository cho các mẫu code

Hãy bắt đầu! 🚀
