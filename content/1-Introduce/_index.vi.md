---
title : "Giới thiệu"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---

#### Tổng quan

VPC Flow Logs là một tính năng cho phép bạn giám sát thông tin về lưu lượng IP đến và đi từ các giao diện mạng trong VPC của bạn. Dữ liệu nhật ký luồng có thể được xuất bản lên Amazon CloudWatch Logs hoặc Amazon S3. Sau khi tạo nhật ký luồng, bạn có thể truy xuất và xem dữ liệu của nó ở điểm đến đã chọn.

Nhật ký luồng có thể giúp bạn thực hiện một số tác vụ, chẳng hạn như:

- Chẩn đoán các quy tắc security group quá hạn chế
- Theo dõi lưu lượng truy cập đến EC2 instance của bạn
- Xác định hướng của lưu lượng truy cập đến và đi từ các giao diện mạng
- Dữ liệu nhật ký luồng được thu thập bên ngoài đường dẫn lưu lượng mạng của bạn và do đó không ảnh hưởng đến lưu lượng hoặc độ trễ của mạng. Bạn có thể tạo hoặc xóa nhật ký luồng mà không có bất kỳ nguy cơ ảnh hưởng nào đến hiệu suất mạng.

Trong lab này, dữ liệu Luồng sẽ được xuất bản lên Amazon CloudWatch Logs.

![Network Monitoring](/images/1/0000.png?featherlight=false&width=50pc)