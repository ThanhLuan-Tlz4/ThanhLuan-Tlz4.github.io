---
title: "Worklog Tuần 6"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:

* Hiểu các dịch vụ lưu trữ và bảo vệ dữ liệu trên AWS.
* Tìm hiểu Amazon S3, AWS Storage Gateway, Snow Family, Disaster Recovery và AWS Backup.
* Hiểu quy trình sao lưu, phục hồi dữ liệu và di chuyển máy ảo lên AWS.
* Thực hành triển khai AWS Backup và VM Import/Export.
* Nâng cao kiến thức thông qua AWS Event Meeting và trao đổi kinh nghiệm với cộng đồng.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | --------------- |
| 2 | - Học lý thuyết về **Amazon S3, Amazon Storage Gateway, Snow Family, Disaster Recovery on AWS và AWS Backup**.<br>- Tìm hiểu các trường hợp sử dụng và kiến trúc triển khai của từng dịch vụ.<br>- Thực hành **Workshop Deploy AWS Backup to the System**: tạo Backup Vault, Backup Plan, Resource Assignment và thực hiện Backup/Restore tài nguyên. | **25/05/2026** | **25/05/2026** | https://www.youtube.com/watch?v=hsCfP0IxoaM&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=103<br>https://000013.awsstudygroup.com/ |
| 3 | - **Workshop VM Import/Export:**<br>&emsp;+ Tìm hiểu quy trình chuyển máy ảo từ On-premises lên AWS.<br>&emsp;+ Chuẩn bị Image và IAM Role.<br>&emsp;+ Thực hiện Import Virtual Machine thành Amazon Machine Image (AMI).<br>&emsp;+ Kiểm tra kết quả sau khi Import. | **26/05/2026** | **26/05/2026** | https://000014.awsstudygroup.com/ |
| 4 | - Tiếp tục thực hành VM Import/Export.<br>&emsp;+ Khởi tạo EC2 từ AMI đã Import.<br>&emsp;+ Kiểm tra hệ điều hành và cấu hình sau khi chuyển đổi.<br>&emsp;+ Thực hiện Export Image và Cleanup tài nguyên. | **27/05/2026** | **27/05/2026** | https://000014.awsstudygroup.com/ |
| 5 | - Ôn tập các nội dung đã học.<br>&emsp;+ So sánh Amazon S3, Storage Gateway, Snow Family và AWS Backup.<br>&emsp;+ Tổng hợp các trường hợp sử dụng trong thực tế.<br>&emsp;+ Đánh giá ưu điểm của VM Import/Export trong Hybrid Cloud. | **28/05/2026** | **28/05/2026** | Tổng hợp tài liệu Workshop |
| 6 | - Thực hành tổng hợp.<br>&emsp;+ Kiểm tra quy trình Backup và Restore.<br>&emsp;+ Đánh giá khả năng di chuyển hệ thống từ On-premises lên AWS bằng VM Import/Export.<br>&emsp;+ Cleanup toàn bộ tài nguyên sau khi hoàn thành các Lab. | **29/05/2026** | **29/05/2026** | https://000013.awsstudygroup.com/<br>https://000014.awsstudygroup.com/ |
| 7 | **AWS EVENT MEETING**<br>- Tham gia buổi chia sẻ và thảo luận cùng cộng đồng AWS.<br>- Trao đổi các chủ đề:<br>&emsp;+ Cách sử dụng AWS hiệu quả.<br>&emsp;+ Giới thiệu chương trình Hackathon AWS.<br>&emsp;+ Nỗi sợ khi mới bắt đầu học Cloud và thiếu tự tin.<br>&emsp;+ Giới thiệu sản phẩm **Tử Vi Đại Việt** và quá trình phát triển trên AWS.<br>&emsp;+ Kinh nghiệm làm việc nhóm trong dự án thực tế.<br>&emsp;+ Phương pháp vượt qua sự trì hoãn và duy trì động lực học tập. | **30/05/2026** | **30/05/2026** | AWS Event Meeting |

---

### Kết quả đạt được tuần 6:

* Hiểu được vai trò của Amazon S3 trong việc lưu trữ dữ liệu dạng Object, đồng thời nắm được mối liên hệ giữa Amazon S3 với AWS Storage Gateway, AWS Backup và các giải pháp Disaster Recovery trong hệ sinh thái AWS.

* Nắm được kiến trúc và trường hợp sử dụng của Amazon Storage Gateway, Snow Family và Disaster Recovery on AWS, từ đó hiểu cách AWS hỗ trợ xây dựng các mô hình Hybrid Cloud và bảo vệ dữ liệu doanh nghiệp.

* Triển khai thành công AWS Backup, tạo Backup Vault, Backup Plan và Resource Assignment để tự động sao lưu tài nguyên AWS theo chính sách đã cấu hình.

* Thực hiện Backup và Restore thành công tài nguyên thông qua AWS Backup, kiểm tra Recovery Point và xác minh khả năng khôi phục dữ liệu sau khi xảy ra sự cố.

* Thực hành thành công VM Import/Export, chuẩn bị máy ảo từ môi trường On-premises, Import thành Amazon Machine Image (AMI) và khởi tạo Amazon EC2 từ AMI đã chuyển đổi.

* Kiểm tra được tính toàn vẹn của hệ điều hành và cấu hình sau quá trình Import, qua đó hiểu được quy trình di chuyển hạ tầng truyền thống lên AWS mà không cần cài đặt lại hệ thống.

* Đánh giá được ưu điểm của VM Import/Export trong quá trình Migration, giúp tận dụng các máy ảo hiện có để triển khai trên môi trường AWS, giảm thời gian và chi phí chuyển đổi.

* Hoàn thành toàn bộ các bài thực hành, thực hiện Cleanup tài nguyên sau khi kết thúc Lab nhằm đảm bảo môi trường AWS không phát sinh chi phí không cần thiết.

* Tham gia AWS Event Meeting, trao đổi với cộng đồng về phương pháp học AWS, kinh nghiệm tham gia Hackathon, kỹ năng làm việc nhóm, cách vượt qua tâm lý thiếu tự tin và sự trì hoãn trong học tập, đồng thời có thêm góc nhìn thực tế về việc phát triển sản phẩm trên nền tảng AWS.