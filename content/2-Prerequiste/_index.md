---
title: "Preparation"
date: "`r Sys.Date()`"
weight: 2
chapter: false
pre: "<b> 2. </b>"
---

#### Preparation 

To implement the infrastructure for this lab, we will use a **[CloudFormation template](https://raw.githubusercontent.com/AWS-First-Cloud-Journey/VPC-Flow-Logs-Template/main/vpc-template.yml)**.

1. Login to the **AWS Management Console**.
   - Find **CloudFormation**.
   - Select **CloudFormation**.

   ![Network Monitoring](/images/0/0001.png?featherlight=false&width=90pc)

2. In the **CloudFormation** interface:
   - Select **Create stack**.
   - Select **With new resources**.

   ![Network Monitoring](/images/0/0002.png?featherlight=false&width=90pc)

3. In the **Create stack** interface:
   - Select **Template is ready**.
   - Select **Upload a template file**.
   - Select **vpc-template.yml**.
   - Select **Next**.

   ![Network Monitoring](/images/0/0003.png?featherlight=false&width=90pc)

4. For the Stack name, enter `VPC`.
   - Select **Next**.

   ![Network Monitoring](/images/0/0004.png?featherlight=false&width=90pc)

5. Select **Next**.

   ![Network Monitoring](/images/0/0005.png?featherlight=false&width=90pc)

6. Select **Create stack**.

   ![Network Monitoring](/images/0/0006.png?featherlight=false&width=90pc)

7. Stack creation successful.

   ![Network Monitoring](/images/0/0007.png?featherlight=false&width=90pc)
