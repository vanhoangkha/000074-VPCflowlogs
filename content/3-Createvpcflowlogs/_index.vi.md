---
title: "Các bước chuẩn bị"
date: "`r Sys.Date()`"
weight: 2
chapter: false
pre: "<b> 2. </b>"
---

#### Các bước chuẩn bị

Để thực hiện triển khai hạ tầng cho bài lab này, chúng ta sẽ sử dụng **[CloudFormation template](https://raw.githubusercontent.com/AWS-First-Cloud-Journey/VPC-Flow-Logs-Template/main/vpc-template.yml)**

1. Đăng nhập vào **AWS Management Console**
   - Tìm **CloudFormation**
   - Chọn **CloudFormation**

   ![Network Monitoring](/images/0/0001.png?featherlight=false&width=90pc)

2. Trong giao diện **CloudFormation**
   - Chọn **Create stack**
   - Chọn **With new resources**

   ![Network Monitoring](/images/0/0002.png?featherlight=false&width=90pc)

3. Trong giao diện **Create stack**
   - Chọn **Template is ready**
   - Chọn **Upload a template file**
   - Chọn **vpc-template.yml**
   - Chọn **Next**

   ![Network Monitoring](/images/0/0003.png?featherlight=false&width=90pc)

4. Đối với Stack name, nhập **`VPC`**
   - Chọn **Next**

   ![Network Monitoring](/images/0/0004.png?featherlight=false&width=90pc)

5. Chọn **Next**

   ![Network Monitoring](/images/0/0005.png?featherlight=false&width=90pc)

6. Chọn **Create stack**

   ![Network Monitoring](/images/0/0006.png?featherlight=false&width=90pc)

7. Tạo Stack thành công.

   ![Network Monitoring](/images/0/0007.png?featherlight=false&width=90pc)
