---
title: "Introduction"
date: "`r Sys.Date()`"
weight: 1
chapter: false
pre: "<b> 1. </b>"
---

#### Overview

VPC Flow Logs is a feature that enables you to capture information about the IP traffic going to and from network interfaces in your VPC. Flow log data can be published to Amazon CloudWatch Logs or Amazon S3. After you create a flow log, you can retrieve and view its data in the chosen destination.

Flow logs can help you with a number of tasks, such as:

- Diagnosing overly restrictive security group rules
- Monitoring the traffic that is reaching your instance
- Determining the direction of the traffic to and from the network interfaces
- Flow log data is collected outside of the path of your network traffic, and therefore does not affect network throughput or latency. You can create or delete flow logs without any risk of impact to network performance.

In this lab, Flow data will be published to Amazon CloudWatch Logs.

![Network Monitoring](/images/1/0000.png?featherlight=false&width=50pc)
