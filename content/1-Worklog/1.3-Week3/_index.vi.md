---

title: "Worklog Tuần 3"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
----------------------

### Mục tiêu tuần 3:

* Hiểu các khái niệm nền tảng về mạng máy tính và kiến trúc mạng trên AWS.
* Nắm được mô hình Amazon Virtual Private Cloud (Amazon VPC) và các thành phần chính.
* Hiểu cách hoạt động của Public Subnet, Private Subnet, Route Table, Internet Gateway, NAT Gateway và Elastic IP.
* Phân biệt Security Group và Network ACL trong việc kiểm soát lưu lượng mạng.
* Thực hành xây dựng một hạ tầng mạng hoàn chỉnh trên AWS và kiểm tra kết nối giữa các thành phần.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                        |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | --------------------------------------------------------------------- |
| 2   | **Networking Fundamentals**<br>- Ôn tập kiến thức mạng cơ bản: IP Address, CIDR, Subnet Mask.<br>- Mô hình TCP/IP, giao thức TCP và UDP.<br>- DNS, HTTP/HTTPS và nguyên lý truyền dữ liệu trên mạng.<br>- Kiến trúc mạng trong môi trường Cloud.                                                            | 04/05/2026   | 04/05/2026      | https://000010.awsstudygroup.com/                                     |
| 3   | **Amazon VPC - Lý thuyết**<br>- Tổng quan Amazon VPC.<br>- Region, Availability Zone (AZ).<br>- CIDR Block, IPv4.<br>- Public Subnet và Private Subnet.<br>- Route Table và Internet Gateway (IGW).                                                                                                         | 05/05/2026   | 05/05/2026      | https://00003.awsstudygroup.com/                                      |
| 4   | **Amazon VPC - Thực hành cơ bản**<br>- Tạo VPC.<br>- Tạo Public Subnet và Private Subnet.<br>- Tạo và cấu hình Route Table.<br>- Gắn Internet Gateway cho VPC.<br>- Kiểm tra kết nối Internet của Public Subnet.                                                                                            | 06/05/2026   | 06/05/2026      | https://00003.awsstudygroup.com/                                      |
| 5   | **Amazon VPC - Thực hành nâng cao**<br>- Tạo Elastic IP.<br>- Triển khai NAT Gateway.<br>- Cấu hình Route Table cho Private Subnet.<br>- Tìm hiểu Security Group và Network ACL.<br>- So sánh Stateful và Stateless Firewall.                                                                               | 07/05/2026   | 07/05/2026      | https://00003.awsstudygroup.com/                                      |
| 6   | **Thực hành tổng hợp**<br>- Hoàn thiện kiến trúc mạng Amazon VPC.<br>- Triển khai EC2 tại Public và Private Subnet.<br>- Kiểm tra SSH, HTTP, ICMP.<br>- Kiểm tra truy cập Internet từ Private Subnet thông qua NAT Gateway.<br>- Ôn tập và tổng kết toàn bộ nội dung Networking Fundamentals và Amazon VPC. | 08/05/2026   | 08/05/2026      | https://00003.awsstudygroup.com/<br>https://000010.awsstudygroup.com/ |

---

### Kết quả đạt được tuần 3:

* Hiểu được các kiến thức nền tảng về mạng máy tính, bao gồm địa chỉ IP, CIDR, Subnet, TCP/IP, DNS, HTTP/HTTPS và nguyên lý truyền dữ liệu trong môi trường Cloud.

* Nắm được kiến trúc mạng trên AWS và vai trò của Amazon Virtual Private Cloud (Amazon VPC) trong việc xây dựng hạ tầng mạng an toàn.

* Hiểu và áp dụng được các thành phần quan trọng của Amazon VPC, bao gồm:

  * Virtual Private Cloud (VPC)
  * CIDR Block
  * Public Subnet
  * Private Subnet
  * Route Table
  * Internet Gateway (IGW)
  * NAT Gateway
  * Elastic IP

* Hiểu được cơ chế định tuyến và luồng truy cập Internet của EC2 trong Public Subnet và Private Subnet.

* Triển khai thành công một hệ thống Amazon VPC với nhiều Subnet, cấu hình đầy đủ Internet Gateway, Route Table và NAT Gateway.

* Phân biệt được Security Group và Network ACL, đồng thời áp dụng để kiểm soát lưu lượng mạng theo từng lớp bảo mật.

* Kiểm tra và xác minh thành công các kết nối:

  * SSH.
  * HTTP.
  * ICMP (Ping).
  * Truy cập Internet từ Public Subnet.
  * Truy cập Internet từ Private Subnet thông qua NAT Gateway.

* Có khả năng thiết kế và triển khai một hạ tầng mạng AWS theo mô hình nhiều lớp (Multi-tier Architecture), tạo nền tảng cho các nội dung nâng cao như Elastic Load Balancing (ELB), Auto Scaling, Hybrid Networking và các kiến trúc Cloud trong những tuần tiếp theo.
