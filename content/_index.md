---
title : "Monitoring network infrastructure"
date : "`r Sys.Date()`"
weight : 1
chapter : false
---
# Monitor network infrastructure

#### Overview

VPC Flow Logs is a feature that allows you to monitor information about IP traffic to and from network interfaces in your VPC. Stream log data can be published to Amazon CloudWatch Logs or Amazon S3. After creating a stream log, you can retrieve and view its data at the selected destination.

{{< figure src="/images/serviceicon.png" title="VPC Flow Logs" width=150pc >}}

Stream logs can help you with several tasks, such as:

- Diagnose security group rules that are too restrictive
- Monitor traffic to your EC2 instance
- Determine the direction of traffic to and from network interfaces
- Flow log data is collected outside your network traffic path and therefore has no impact on network traffic or latency. You can create or delete stream logs without risk affecting network performance.

In this lab, Stream data will be published to Amazon CloudWatch Logs.

![Network Monitoring](/images/1/0000.png?featherlight=false&width=50pc)

#### Content

1. [Introduction](1-introduce/)
2. [Preparation steps](2-prerequiste/)
3. [Create VPC Flow Logs](3-createvpcflowlogs/)
4. [Enable VPC Flow Logs](4-enablevpcflowlogs/)
5. [Network Monitoring](5-monitoring/)
6. [Resource Cleanup](6-cleanup/)