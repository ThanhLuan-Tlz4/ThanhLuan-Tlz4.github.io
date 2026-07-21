---
title: "Worklog Tuần 7"
date: 2024-01-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

* Ôn tập các kiến thức đã học về dịch vụ lưu trữ trên AWS.
* Hiểu kiến trúc và trường hợp sử dụng của Amazon FSx for Windows File Server.
* Thực hành triển khai hệ thống File Server được quản lý trên AWS.
* Củng cố kiến thức về Amazon S3 thông qua các bài thực hành.
* So sánh các giải pháp lưu trữ Amazon S3, Amazon FSx và AWS Storage Gateway.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | --------------- |
| 2 | - Ôn tập các kiến thức về Amazon S3, AWS Storage Gateway, AWS Backup, VM Import/Export và Disaster Recovery.<br>- **Workshop Amazon FSx for Windows File Server:**<br>&emsp;+ Tìm hiểu kiến trúc và các thành phần của Amazon FSx.<br>&emsp;+ Triển khai File System Windows File Server.<br>&emsp;+ Cấu hình Security Group và kết nối từ Amazon EC2.<br>&emsp;+ Kiểm tra khả năng chia sẻ dữ liệu qua SMB.<br>- **Workshop Starting with Amazon S3:**<br>&emsp;+ Tạo và quản lý S3 Bucket.<br>&emsp;+ Upload, Download và quản lý Object.<br>&emsp;+ Thực hành Static Website Hosting và Bucket Policy. | **01/06/2026** | **01/06/2026** | https://000025.awsstudygroup.com/<br>https://000057.awsstudygroup.com/ |
| 3 | - Tiếp tục thực hành Amazon FSx.<br>&emsp;+ Tạo Shared Folder.<br>&emsp;+ Phân quyền truy cập File Share.<br>&emsp;+ Kiểm tra khả năng đọc/ghi dữ liệu từ EC2 Windows.<br>&emsp;+ Đánh giá hiệu năng của File Server được quản lý. | **02/06/2026** | **02/06/2026** | https://000025.awsstudygroup.com/ |
| 4 | - Tiếp tục thực hành Amazon S3.<br>&emsp;+ Quản lý Bucket Policy và Block Public Access.<br>&emsp;+ Thực hành Versioning.<br>&emsp;+ Kiểm tra truy cập Website Endpoint.<br>&emsp;+ Thực hiện Cleanup tài nguyên. | **03/06/2026** | **03/06/2026** | https://000057.awsstudygroup.com/ |
| 5 | - Tổng hợp kiến thức về các dịch vụ lưu trữ AWS.<br>&emsp;+ So sánh Amazon S3, Amazon FSx, AWS Storage Gateway và AWS Backup.<br>&emsp;+ Phân tích trường hợp sử dụng của từng dịch vụ trong doanh nghiệp. | **04/06/2026** | **04/06/2026** | Tổng hợp tài liệu Workshop |
| 6 | - Thực hành tổng hợp.<br>&emsp;+ Kiểm tra kết nối giữa EC2 và Amazon FSx.<br>&emsp;+ Đánh giá cơ chế lưu trữ Object Storage và File Storage trên AWS.<br>&emsp;+ Cleanup toàn bộ tài nguyên sau khi hoàn thành Workshop. | **05/06/2026** | **05/06/2026** | https://000025.awsstudygroup.com/<br>https://000057.awsstudygroup.com/ |
| 7 | **AWS EVENT MEETING**<br>- Tham gia buổi chia sẻ và thảo luận cùng cộng đồng AWS.<br>- Trao đổi các chủ đề:<br>&emsp;+ Cách sử dụng AWS hiệu quả.<br>&emsp;+ Giới thiệu chương trình Hackathon AWS.<br>&emsp;+ Nỗi sợ khi mới bắt đầu học Cloud và thiếu tự tin.<br>&emsp;+ Giới thiệu sản phẩm **Tử Vi Đại Việt** và quá trình phát triển trên AWS.<br>&emsp;+ Kinh nghiệm làm việc nhóm trong dự án thực tế.<br>&emsp;+ Phương pháp vượt qua sự trì hoãn và duy trì động lực học tập. | **06/06/2026** | **06/05/2026** | AWS Event Meeting |
---

### Kết quả đạt được tuần 7:

* Ôn tập và hệ thống lại các kiến thức đã học về Amazon S3, AWS Storage Gateway, AWS Backup, VM Import/Export và Disaster Recovery, từ đó hiểu rõ mối liên hệ giữa các dịch vụ lưu trữ và bảo vệ dữ liệu trên AWS.

* Triển khai thành công Amazon FSx for Windows File Server, tạo File System và cấu hình các thành phần mạng cần thiết để dịch vụ có thể hoạt động trong Amazon VPC.

* Thực hiện kết nối Amazon EC2 đến Amazon FSx thông qua giao thức SMB, tạo Shared Folder và kiểm tra khả năng đọc, ghi và chia sẻ dữ liệu giữa các máy trong cùng hệ thống.

* Hiểu được cách Amazon FSx cung cấp dịch vụ File Server được quản lý hoàn toàn trên AWS, giúp giảm công sức vận hành so với việc tự triển khai Windows File Server truyền thống.

* Thực hành tạo và quản lý Amazon S3 Bucket, thực hiện Upload, Download, xóa và quản lý Object thông qua AWS Management Console.

* Cấu hình thành công Static Website Hosting, Bucket Policy và Block Public Access, đồng thời kiểm tra khả năng truy cập Website Endpoint sau khi cấu hình hoàn tất.

* Thực hành Versioning trên Amazon S3 để theo dõi các phiên bản của Object, từ đó hiểu được cơ chế bảo vệ dữ liệu trước các thao tác ghi đè hoặc xóa nhầm.

* So sánh được sự khác biệt giữa Amazon S3 (Object Storage), Amazon FSx (Managed File Storage), AWS Storage Gateway (Hybrid Storage) và AWS Backup (Data Protection), đồng thời xác định được các trường hợp sử dụng phù hợp của từng dịch vụ trong thực tế.

* Hoàn thành toàn bộ các bài thực hành, thực hiện Cleanup tài nguyên sau khi kết thúc Workshop nhằm đảm bảo không phát sinh chi phí trên tài khoản AWS.