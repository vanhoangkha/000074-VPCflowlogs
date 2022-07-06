---
title : "Tạo VPC Flow Logs"
date :  "`r Sys.Date()`" 
weight : 3
chapter : false
pre : " <b> 3. </b> "
---

#### Tạo VPC Flow Logs

VPC Flow Logs là một tính năng cho phép bạn giám sát thông tin về lưu lượng IP đến và đi từ các giao diện mạng trong VPC của bạn. Dữ liệu nhật ký luồng có thể được xuất bản lên Amazon CloudWatch Logs hoặc Amazon S3. Sau khi tạo nhật ký luồng, bạn có thể truy xuất và xem dữ liệu của nó ở điểm đến đã chọn.

Nhật ký luồng có thể giúp bạn thực hiện một số tác vụ, chẳng hạn như:

- Chẩn đoán các quy tắc security group quá hạn chế
- Theo dõi lưu lượng truy cập đến EC2 instance của bạn
- Xác định hướng của lưu lượng truy cập đến và đi từ các giao diện mạng
- Dữ liệu nhật ký luồng được thu thập bên ngoài đường dẫn lưu lượng mạng của bạn và do đó không ảnh hưởng đến lưu lượng hoặc độ trễ của mạng. Bạn có thể tạo hoặc xóa nhật ký luồng mà không có bất kỳ nguy cơ ảnh hưởng nào đến hiệu suất mạng.

Trong lab này, dữ liệu Luồng sẽ được xuất bản lên Amazon CloudWatch Logs.

#### Sử dụng CloudFormation để triển khai hạ tầng

  - Tạo **IAM Role** để sử dụng đẩy **flow logs** lên **cloudwatch**
  - **Cloud Watch Log Group**, flow log sẽ được đẩy lên group này.
  - **EC2 instance**, sử dụng để kiểm tra lưu lượng

1. Chúng ta phải chuẩn bị 

   - Tải file **[VPC-Flow-Logs-Lab.yaml](https://github.com/AWS-First-Cloud-Journey/VPC-Flow-Logs-Template.git)**
   - Truy cập vào **AWS Management Console**, tìm **CloudFormation**
   - Chọn **CloudFormation**

![Network Monitoring](/images/2/0000.png?featherlight=false&width=90pc)

2. Trong giao diện **AWS CloudFormation**

   - Chọn **Create stack**
   - Chọn **With new resources**

![Network Monitoring](/images/1/0001.png?featherlight=false&width=90pc)

3. Trong giao diện **Create stack**

   - Chọn **Template is ready**
   - Chọn **Upload a template file**
   - Chọn **Choose file**
   - Chọn file yaml đã tải về.
   - Chọn **Next**

![Network Monitoring](/images/1/0002.png?featherlight=false&width=90pc)

4. Trong giao diện **Specify stack details**

   - Nhập **```Network-Monitoring```**
   - Đối với các **Parameters**, chọn **VPC** đã tạo 
   - Chọn **Public subnet** đã tạo
   - Chọn **Next** 

![Network Monitoring](/images/1/0003.png?featherlight=false&width=90pc)

5. Chọn **Next**

![Network Monitoring](/images/1/0004.png?featherlight=false&width=90pc)

6. Chọn **Create stack**

![Network Monitoring](/images/1/0005.png?featherlight=false&width=90pc)

7. Hoàn thành tạo stack

![Network Monitoring](/images/1/0006.png?featherlight=false&width=90pc)

8. Truy cập vào giao diện **EC2**, kiểm tra đã tạo ra 1 EC2 instance.

![Network Monitoring](/images/1/0007.png?featherlight=false&width=90pc)

9. Sử dụng **Public IPv4 DNS** truy cập.

![Network Monitoring](/images/1/0008.png?featherlight=false&width=90pc)


