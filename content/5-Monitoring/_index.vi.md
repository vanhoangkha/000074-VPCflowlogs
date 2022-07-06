---
title : "Giám sát hạ tầng mạng"
date :  "`r Sys.Date()`" 
weight : 5
chapter : false
pre : " <b> 5. </b> "
---

#### Giám sát hạ tầng mạng

Sau khi đã triển khai hạ tầng mạng và kích hoạt VPC Flow Logs. Chúng ta sẽ bắt đầu giám  sát hạ tầng thôi.


1. Truy cập vào **AWS CloudWatch**

    - Chọn **Log groups**
    - Chọn **VPCFlowLogGroup**

![Network Monitoring](/images/3/0001.png?featherlight=false&width=90pc)

2. Trong giao diện **VPCFlowLogGroup**

   - Chọn **Log streams**
   - Chúng ta sẽ thấy có log stream được tạo về ENI

![Network Monitoring](/images/3/0002.png?featherlight=false&width=90pc)

3. Truy cập vào trong log stream vào xem chi tiết Log events.

![Network Monitoring](/images/3/0003.png?featherlight=false&width=90pc)

4. Quay lại giao diện **CloudWatch**

   - Chọn **Log Insights**
   - Thực hiện **Run query**
   - Sau đó quan sát log 

![Network Monitoring](/images/3/0004.png?featherlight=false&width=90pc)

Vậy là chúng ta đã thiết lập giám sát hạ tầng mạng cơ bản. Mong rằng bài lab này sẽ giúp các bạn hiểu rõ hơn về tính năng của **VPC Flow Logs**


