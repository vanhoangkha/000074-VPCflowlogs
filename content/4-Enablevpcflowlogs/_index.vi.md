---
title : "Kích hoạt VPC Flow Logs"
date :  "`r Sys.Date()`" 
weight : 4
chapter : false
pre : " <b> 4. </b> "
---

#### Kích hoạt VPC Flow Logs

1. Truy cập vào giao diện **VPC**

   - Chọn  VPC đã chuẩn bị
   - Chọn **Flow logs**
   - Chọn **Create flow log**

![Network Monitoring](/images/2/0001.png?featherlight=false&width=90pc)

2. Trong giao diện **Create flow log**

   - Thực hiện cấu hình đối với **Filter**, chọn **All**
   - Chọn **Maximum aggregation interval** là 10 minutes
   - **Destination** chọn **Send to CloudWatch Logs**

![Network Monitoring](/images/2/0002.png?featherlight=false&width=90pc)

3. Tiếp tục cấu hình

   - **Destination log group**, chọn **VPCFlowLogGroup** đã tạo từ CloudFormation
   - **IAM Role** chọn **RoleForVPCFlowLogs** đã tạo từ CloudFormation
   - **Log record formation**, chọn **AWS default format**
   - Chọn **Create flow log**

![Network Monitoring](/images/2/0003.png?featherlight=false&width=90pc)

4. Hoàn thành tạo **VPC Flow Logs**

![Network Monitoring](/images/2/0004.png?featherlight=false&width=90pc)

