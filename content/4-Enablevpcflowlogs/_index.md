---
title: "Enable VPC Flow Logs"
date: "`r Sys.Date()`"
weight: 4
chapter: false
pre: "<b>4.</b>"
---

#### Enable VPC Flow Logs

1. Access to the **VPC** interface:

   - Select **VPC**.
   - Select **Flow logs**.
   - Select **Create flow log**.

   ![Network Monitoring](/images/2/0001.png?featherlight=false&width=90pc)

2. In the **Create flow log** interface:

   - Configure the **Filter**, select **All**.
   - Set the **Maximum aggregation interval** to 10 minutes.
   - For **Destination**, select **Send to CloudWatch Logs**.

   ![Network Monitoring](/images/2/0002.png?featherlight=false&width=90pc)

3. Continue with the configuration:

   - For **Destination log group**, select **VPCFlowLogGroup** created from CloudFormation.
   - For **IAM Role**, select **RoleForVPCFlowLogs** created from CloudFormation.
   - In **Log record format**, select **AWS default format**.
   - Select **Create flow log**.

   ![Network Monitoring](/images/2/0003.png?featherlight=false&width=90pc)

4. Complete the creation of **VPC Flow Logs**.

   ![Network Monitoring](/images/2/0004.png?featherlight=false&width=90pc)
