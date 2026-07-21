---
title: "Worklog Tuần 5"
date: 2024-01-01
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:

* Hiểu dịch vụ lưu trữ Amazon S3 và các thành phần cơ bản.
* Tìm hiểu cơ chế sao lưu dữ liệu với AWS Backup.
* Tìm hiểu kiến trúc Hybrid Storage thông qua AWS Storage Gateway.
* Thực hành tạo Bucket, quản lý Object và triển khai Static Website trên Amazon S3.
* Thực hành triển khai Backup Plan, Restore dữ liệu và kết nối File Storage Gateway với môi trường On-premises.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | --------------- |
| 2 | - Tìm hiểu tổng quan về Amazon S3.<br>- Tìm hiểu Bucket, Object, Storage Class và Versioning.<br>- Thực hành tạo S3 Bucket và upload dữ liệu.<br>- Làm quen với các thiết lập bảo mật của Amazon S3. | **18/05/2026** | **18/05/2026** | https://000057.awsstudygroup.com/ |
| 3 | - **Workshop Amazon S3:**<br>&emsp;+ Quản lý Object trong S3 Bucket.<br>&emsp;+ Cấu hình Static Website Hosting.<br>&emsp;+ Thực hành Bucket Policy, Block Public Access và Website Endpoint.<br>&emsp;+ Kiểm tra khả năng truy cập Website từ Internet. | **19/05/2026** | **19/05/2026** | https://000057.awsstudygroup.com/ |
| 4 | - **Workshop AWS Backup:**<br>&emsp;+ Triển khai hạ tầng phục vụ Backup.<br>&emsp;+ Tạo Backup Vault và Backup Plan.<br>&emsp;+ Gán tài nguyên cần sao lưu.<br>&emsp;+ Thực hiện Backup và Restore dữ liệu.<br>&emsp;+ Kiểm tra quá trình Restore và Cleanup tài nguyên. | **20/05/2026** | **20/05/2026** | https://000013.awsstudygroup.com/ |
| 5 | - **Workshop AWS Storage Gateway:**<br>&emsp;+ Chuẩn bị môi trường Storage Gateway.<br>&emsp;+ Triển khai File Storage Gateway trên EC2.<br>&emsp;+ Tạo File Share kết nối với Amazon S3.<br>&emsp;+ Cấu hình SMB và Mount File Share từ máy On-premises. | **21/05/2026** | **21/05/2026** | https://000024.awsstudygroup.com/ |
| 6 | - **Thực hành tổng hợp:**<br>&emsp;+ Kiểm tra đồng bộ dữ liệu giữa On-premises và Amazon S3 thông qua File Storage Gateway.<br>&emsp;+ Đánh giá quy trình Backup và Restore bằng AWS Backup.<br>&emsp;+ So sánh các phương pháp lưu trữ và bảo vệ dữ liệu trên AWS.<br>&emsp;+ Cleanup toàn bộ tài nguyên sau khi hoàn thành Workshop. | **22/05/2026** | **22/05/2026** | https://000013.awsstudygroup.com/<br>https://000024.awsstudygroup.com/<br>https://000057.awsstudygroup.com/ |

---

### Kết quả đạt được tuần 5:

* Hiểu được kiến trúc lưu trữ Object Storage của Amazon S3, nắm được mối quan hệ giữa Bucket, Object, Key, Storage Class và Versioning trong quá trình quản lý dữ liệu trên AWS.

* Triển khai thành công Amazon S3 Bucket, thực hiện upload, download và quản lý các Object thông qua AWS Management Console, đồng thời làm quen với các thao tác quản trị dữ liệu trên S3.

* Cấu hình thành công Static Website Hosting trên Amazon S3, thiết lập Bucket Policy và Website Endpoint để công khai nội dung website, từ đó hiểu được cơ chế hoạt động của dịch vụ lưu trữ tĩnh trên AWS.

* Thực hành cấu hình Block Public Access, Bucket Policy và các thiết lập bảo mật cơ bản của Amazon S3, qua đó hiểu được cách kiểm soát quyền truy cập đối với dữ liệu lưu trữ.

* Triển khai thành công AWS Backup, tạo Backup Vault, Backup Plan và Resource Assignment để tự động sao lưu các tài nguyên AWS theo lịch trình, đồng thời hiểu được cơ chế quản lý và tự động hóa việc sao lưu dữ liệu.

* Thực hiện Backup và Restore thành công tài nguyên thông qua AWS Backup, kiểm tra Recovery Point và xác minh khả năng khôi phục dữ liệu, từ đó hiểu được quy trình bảo vệ dữ liệu và phục hồi khi xảy ra sự cố.

* Triển khai File Storage Gateway trên Amazon EC2, tạo File Share liên kết với Amazon S3 và cấu hình giao thức SMB để cung cấp vùng lưu trữ dùng chung cho môi trường On-premises.

* Thực hiện Mount File Share từ máy On-premises, kiểm tra quá trình đồng bộ dữ liệu giữa hệ thống cục bộ và Amazon S3, qua đó hiểu được cơ chế Hybrid Storage và cách AWS Storage Gateway kết nối hạ tầng truyền thống với dịch vụ lưu trữ trên Cloud.

* Đánh giá được vai trò của Amazon S3, AWS Backup và AWS Storage Gateway trong việc xây dựng hệ thống lưu trữ, sao lưu và đồng bộ dữ liệu trên AWS, đồng thời hoàn thành Cleanup toàn bộ tài nguyên sau khi kết thúc các bài thực hành nhằm tránh phát sinh chi phí.