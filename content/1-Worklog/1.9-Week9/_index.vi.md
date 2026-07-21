---
title: "Worklog Tuần 9"
date: 2024-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu tuần 9:

* Củng cố kiến thức về các dịch vụ bảo mật và quản lý truy cập trên AWS.
* Hiểu cách kiểm soát quyền truy cập tài nguyên EC2 thông qua IAM Policy kết hợp Resource Tags.
* Tìm hiểu cơ chế giới hạn quyền của IAM User và IAM Role bằng IAM Permission Boundary.
* Thực hành mã hóa dữ liệu lưu trữ bằng AWS Key Management Service (AWS KMS).
* Nâng cao khả năng thiết kế hệ thống bảo mật theo nguyên tắc Least Privilege trên AWS.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | --------------- |
| 2 | - Học lý thuyết về **Shared Responsibility Model**, **IAM**, **Amazon Cognito**, **AWS Organizations**, **IAM Identity Center (SSO)** và **AWS KMS** nhằm củng cố kiến thức bảo mật AWS.<br>- **Workshop Manage Access to EC2 Services with Resource Tags through IAM Services:**<br>&emsp;+ Tìm hiểu cơ chế kiểm soát quyền truy cập bằng Resource Tags.<br>&emsp;+ Tạo IAM Policy sử dụng điều kiện Tag.<br>&emsp;+ Kiểm tra quyền truy cập EC2 theo từng nhóm tài nguyên. | **15/06/2026** | **15/06/2026** | https://www.youtube.com/watch?v=tsobAlSg19g&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=150<br>https://000028.awsstudygroup.com/ |
| 3 | - **Workshop Limitation of User Rights with IAM Permission Boundary:**<br>&emsp;+ Tìm hiểu nguyên lý hoạt động của Permission Boundary.<br>&emsp;+ Tạo IAM Policy Boundary.<br>&emsp;+ Áp dụng Permission Boundary cho IAM User và IAM Role.<br>&emsp;+ Kiểm tra giới hạn quyền truy cập sau khi cấu hình. | **16/06/2026** | **16/06/2026** | https://000030.awsstudygroup.com/ |
| 4 | - **Workshop Encrypt at Rest with AWS KMS:**<br>&emsp;+ Tạo Customer Managed Key (CMK).<br>&emsp;+ Cấu hình mã hóa dữ liệu bằng AWS KMS.<br>&emsp;+ Kiểm tra quyền sử dụng KMS Key.<br>&emsp;+ Thực hành mã hóa tài nguyên lưu trữ trên AWS. | **17/06/2026** | **17/06/2026** | https://000033.awsstudygroup.com/ |
| 5 | - Tổng hợp kiến thức về IAM và AWS KMS.<br>&emsp;+ So sánh IAM Policy, Resource Tags và Permission Boundary.<br>&emsp;+ Phân tích các mô hình phân quyền theo nguyên tắc Least Privilege.<br>&emsp;+ Đánh giá vai trò của AWS KMS trong việc bảo vệ dữ liệu trên Cloud. | **18/06/2026** | **18/06/2026** | Tổng hợp tài liệu Workshop |
| 6 | - Thực hành tổng hợp.<br>&emsp;+ Kiểm tra quyền truy cập EC2 theo Resource Tags.<br>&emsp;+ Kiểm tra hiệu lực của Permission Boundary.<br>&emsp;+ Xác minh dữ liệu được mã hóa bằng AWS KMS.<br>&emsp;+ Cleanup toàn bộ tài nguyên sau khi hoàn thành Workshop. | **19/06/2026** | **19/06/2026** | https://000028.awsstudygroup.com/<br>https://000030.awsstudygroup.com/<br>https://000033.awsstudygroup.com/ |

---

### Kết quả đạt được tuần 9:

* Củng cố kiến thức về các dịch vụ bảo mật trên AWS, hiểu rõ mối quan hệ giữa IAM, Resource Tags, Permission Boundary và AWS KMS trong việc xây dựng hệ thống phân quyền và bảo vệ dữ liệu.

* Thực hành thành công việc quản lý quyền truy cập Amazon EC2 thông qua **IAM Policy kết hợp Resource Tags**, tạo các chính sách sử dụng điều kiện (`Condition`) để chỉ cho phép người dùng thao tác trên các EC2 Instance có Tag phù hợp.

* Kiểm tra và xác minh quyền truy cập của nhiều IAM User với các tài nguyên được gắn Tag khác nhau, từ đó hiểu được cách triển khai mô hình phân quyền theo từng dự án hoặc từng phòng ban mà không cần tạo nhiều IAM Policy riêng biệt.

* Triển khai thành công **IAM Permission Boundary**, tạo Permission Boundary Policy và áp dụng cho IAM User hoặc IAM Role nhằm giới hạn phạm vi quyền tối đa mà các đối tượng này có thể được cấp.

* Thực hiện kiểm tra các trường hợp quyền được cấp vượt quá Permission Boundary, qua đó hiểu được cách Permission Boundary hoạt động như một lớp kiểm soát bổ sung nhằm ngăn chặn việc cấp quyền ngoài phạm vi cho phép.

* Tạo thành công **Customer Managed Key (CMK)** bằng AWS Key Management Service (AWS KMS), quản lý quyền sử dụng khóa mã hóa và thực hành mã hóa dữ liệu lưu trữ trên các dịch vụ AWS.

* Hiểu được cơ chế **Encrypt at Rest** trên AWS, nắm được cách AWS KMS quản lý khóa mã hóa, thực hiện mã hóa và giải mã dữ liệu một cách an toàn mà vẫn đảm bảo khả năng kiểm soát quyền truy cập.

* Đánh giá được hiệu quả của việc kết hợp Resource Tags, IAM Policy, Permission Boundary và AWS KMS trong việc xây dựng hệ thống bảo mật theo nguyên tắc **Least Privilege**, giúp tăng cường khả năng kiểm soát truy cập và bảo vệ dữ liệu trên nền tảng AWS.

* Hoàn thành toàn bộ các bài thực hành, thực hiện Cleanup tài nguyên sau khi kết thúc Workshop nhằm đảm bảo môi trường AWS không phát sinh chi phí ngoài mong muốn.