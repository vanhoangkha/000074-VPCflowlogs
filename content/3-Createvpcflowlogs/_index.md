---
title: "Create VPC Flow Logs"
date: "`r Sys.Date()`"
weight: 3
chapter: false
pre: "<b>3.</b>"
---

#### Create VPC Flow Logs

VPC Flow Logs is a feature that allows you to monitor information about IP traffic to and from network interfaces in your VPC. Stream log data can be published to Amazon CloudWatch Logs or Amazon S3. After creating a stream log, you can retrieve and view its data at the selected destination.

Stream logs can help you with several tasks, such as:

- Diagnose security group rules that are too restrictive
- Monitor traffic to your EC2 instance
- Determine the direction of traffic to and from network interfaces
- Flow log data is collected outside your network traffic path and therefore has no impact on network traffic or latency. You can create or delete stream logs without the risk of affecting network performance.

In this lab, Stream data will be published to Amazon CloudWatch Logs.

#### Using CloudFormation to deploy infrastructure

- Create **IAM Role** to use to push **flow logs** to **cloudwatch**
- **Cloud Watch Log Group**, the flow log will be pushed to this group.
- **EC2 instance**, used to check traffic

1. We must prepare
   - Download file **[VPC-Flow-Logs-Lab.yaml](https://github.com/AWS-First-Cloud-Journey/VPC-Flow-Logs-Template.git)**
   - Go to **AWS Management Console**, find **CloudFormation**
   - Select **CloudFormation**

   ![Network Monitoring](/images/2/0000.png?featherlight=false&width=90pc)

2. In the **AWS CloudFormation** interface
   - Select **Create stack**
   - Select **With new resources**

   ![Network Monitoring](/images/1/0001.png?featherlight=false&width=90pc)

3. In the **Create stack** interface
   - Select **Template is ready**
   - Select **Upload a template file**
   - Select **Choose file**
   - Select the downloaded yaml file.
   - Select **Next**

   ![Network Monitoring](/images/1/0002.png?featherlight=false&width=90pc)

4. In the **Specify stack details** interface
   - Enter **`Network-Monitoring`**
   - For **Parameters**, select the created **VPC**
   - Select **Public subnet** created
   - Select **Next**

   ![Network Monitoring](/images/1/0003.png?featherlight=false&width=90pc)

5. Select **Next**

   ![Network Monitoring](/images/1/0004.png?featherlight=false&width=90pc)

6. Select **Create stack**

   ![Network Monitoring](/images/1/0005.png?featherlight=false&width=90pc)

7. Complete stack creation

   ![Network Monitoring](/images/1/0006.png?featherlight=false&width=90pc)

8. Access to **EC2** interface, the test created 1 EC2 instance.

   ![Network Monitoring](/images/1/0007.png?featherlight=false&width=90pc)

9. Use **Public IPv4 DNS** to access.

   ![Network Monitoring](/images/1/0008.png?featherlight=false&width=90pc)
