---
title : "Network infrastructure monitoring"
date : "`r Sys.Date()`"
weight : 5
chapter : false
pre : " <b> 5. </b> "
---

#### Network infrastructure monitoring

After deploying the network infrastructure and activating VPC Flow Logs. We'll start monitoring the infrastructure.


1. Access to **AWS CloudWatch**

    - Select **Log groups**
    - Select **VPCFlowLogGroup**

![Network Monitoring](/images/3/0001.png?featherlight=false&width=90pc)

2. In the **VPCFlowLogGroup** interface

   - Select **Log streams**
   - We will see a log stream created about ENI

![Network Monitoring](/images/3/0002.png?featherlight=false&width=90pc)

3. Access the log stream to view the details of Log events.

![Network Monitoring](/images/3/0003.png?featherlight=false&width=90pc)

4. Return to **CloudWatch** interface

   - Select **Log Insights**
   - Execute **Run query**
   - Then observe the log

![Network Monitoring](/images/3/0004.png?featherlight=false&width=90pc)

So we have set up basic network infrastructure monitoring. Hope this lab will help you better understand the features of **VPC Flow Logs**