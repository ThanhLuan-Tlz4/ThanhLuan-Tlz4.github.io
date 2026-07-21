---
title: "Worklog Tuần 2"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu tuần 2:

* Hiểu cơ chế quản lý danh tính và phân quyền trên AWS thông qua dịch vụ AWS Identity and Access Management (IAM).
* Nắm được cách hoạt động của IAM User, Group, Role và Policy.
* Thực hành sử dụng AWS CLI để quản lý tài nguyên AWS.
* Áp dụng nguyên tắc Least Privilege nhằm xây dựng môi trường AWS an toàn.
* Hoàn thành các bài thực hành về IAM và AWS CLI trong chương trình First Cloud AI Journey.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | --------------- |
| 2 | - Tìm hiểu AWS Identity and Access Management (IAM).<br>- Khái niệm Authentication và Authorization.<br>- Root User và IAM User.<br>- Shared Responsibility Model. | **27/04/2026** | **27/04/2026** | https://000002.awsstudygroup.com/ |
| 3 | - Tìm hiểu IAM User, IAM Group, Managed Policy và Inline Policy.<br>- **Thực hành:**<br>&emsp;+ Tạo IAM User.<br>&emsp;+ Tạo IAM Group.<br>&emsp;+ Gán Policy cho User và Group.<br>&emsp;+ Kiểm tra quyền truy cập. | **28/04/2026** | **28/04/2026** | https://000002.awsstudygroup.com/2-iam-user/ |
| 4 | - Tìm hiểu IAM Role và AWS STS.<br>- **Thực hành:**<br>&emsp;+ Tạo IAM Role cho Amazon EC2.<br>&emsp;+ Gán Role cho EC2 Instance.<br>&emsp;+ Kiểm tra quyền truy cập Amazon S3 thông qua IAM Role. | **29/04/2026** | **29/04/2026** | https://000002.awsstudygroup.com/3-iam-role/ |
| 5 | - Tìm hiểu AWS CLI và xác thực bằng IAM Credentials.<br>- **Thực hành:**<br>&emsp;+ aws configure.<br>&emsp;+ aws sts get-caller-identity.<br>&emsp;+ aws iam list-users.<br>&emsp;+ aws ec2 describe-instances.<br>&emsp;+ aws s3 ls. | **30/04/2026** | **30/04/2026** | https://000010.awsstudygroup.com/ |
| 6 | - **Thực hành tổng hợp:**<br>&emsp;+ Xây dựng mô hình IAM hoàn chỉnh gồm User, Group, Role và Policy.<br>&emsp;+ Thực hiện quản lý tài nguyên bằng cả AWS Management Console và AWS CLI.<br>&emsp;+ Kiểm tra quyền theo nguyên tắc Least Privilege. | **01/05/2026** | **02/05/2026** | https://000002.awsstudygroup.com/ |

---

### Kết quả đạt được tuần 2:

* Hiểu được mô hình quản lý danh tính và phân quyền của AWS thông qua dịch vụ AWS Identity and Access Management (IAM).

* Nắm được chức năng và cách sử dụng của:
  * IAM User.
  * IAM Group.
  * IAM Role.
  * Managed Policy.
  * Inline Policy.

* Hiểu và áp dụng nguyên tắc **Least Privilege** trong quá trình cấp quyền cho người dùng và dịch vụ.

* Thực hành thành công việc tạo và quản lý nhiều IAM User, IAM Group và IAM Role phục vụ cho các tình huống quản trị hệ thống.

* Hiểu cơ chế xác thực tạm thời thông qua IAM Role và AWS Security Token Service (STS).

* Sử dụng AWS CLI để thực hiện các thao tác quản trị cơ bản như:
  * Kiểm tra thông tin tài khoản AWS.
  * Liệt kê IAM Users.
  * Kiểm tra EC2 Instances.
  * Liệt kê các S3 Bucket.
  * Xác minh thông tin người dùng hiện tại bằng `aws sts get-caller-identity`.

* Có khả năng kết hợp AWS Management Console và AWS CLI để quản lý tài nguyên AWS một cách hiệu quả.

* Xây dựng được mô hình phân quyền cơ bản theo nguyên tắc bảo mật của AWS, tạo nền tảng cho các bài thực hành về Amazon VPC và Networking ở các tuần tiếp theo.