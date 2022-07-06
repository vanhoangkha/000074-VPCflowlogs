---
title : "Enable VPC Flow Logs"
date : "`r Sys.Date()`"
weight : 4
chapter : false
pre : " <b> 4. </b> "
---

#### Enable VPC Flow Logs

1. Access to **VPC** interface

   - Select **VPC**
   - Select **Flow logs**
   - Select **Create flow log**

![Network Monitoring](/images/2/0001.png?featherlight=false&width=90pc)

2. In the **Create flow log** interface

   - Make configuration for **Filter**, select **All**
   - Set **Maximum aggregation interval** to 10 minutes
   - **Destination** select **Send to CloudWatch Logs**

![Network Monitoring](/images/2/0002.png?featherlight=false&width=90pc)

3. Continue configuration

   - **Destination log group**, select **VPCFlowLogGroup** created from CloudFormation
   - **IAM Role** select **RoleForVPCFlowLogs** created from CloudFormation
   - **Log record formation**, select **AWS default format**
   - Select **Create flow log**

![Network Monitoring](/images/2/0003.png?featherlight=false&width=90pc)

4. Complete creation of **VPC Flow Logs**

![Network Monitoring](/images/2/0004.png?featherlight=false&width=90pc)