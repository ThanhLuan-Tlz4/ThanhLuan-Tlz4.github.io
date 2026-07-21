---
title: "Worklog Tuần 8"
date: 2024-01-01
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8:

* Hiểu mô hình Shared Responsibility Model trên AWS.
* Tìm hiểu các dịch vụ quản lý danh tính và bảo mật như IAM, Amazon Cognito, AWS Organizations, IAM Identity Center và AWS KMS.
* Thực hành sử dụng AWS Security Hub để giám sát tình trạng bảo mật.
* Tìm hiểu cách tối ưu chi phí Amazon EC2 bằng AWS Lambda.
* Thực hành quản lý tài nguyên AWS bằng Tags và Resource Groups.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | --------------- |
| 2 | - Học lý thuyết về **Shared Responsibility Model**, **AWS IAM**, **Amazon Cognito**, **AWS Organizations**, **IAM Identity Center (SSO)** và **AWS KMS**.<br>- Tìm hiểu vai trò của từng dịch vụ trong việc quản lý danh tính, phân quyền và bảo mật dữ liệu trên AWS.<br>- **Workshop Getting Started with AWS Security Hub:**<br>&emsp;+ Kích hoạt AWS Security Hub.<br>&emsp;+ Phân tích các Security Standards và Findings.<br>&emsp;+ Đánh giá tình trạng bảo mật của tài khoản AWS. | **08/06/2026** | **08/06/2026** | https://www.youtube.com/watch?v=tsobAlSg19g&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=150<br>https://000018.awsstudygroup.com/ |
| 3 | - **Workshop Optimizing EC2 Costs with Lambda:**<br>&emsp;+ Tìm hiểu giải pháp tối ưu chi phí EC2.<br>&emsp;+ Tạo AWS Lambda để tự động Start/Stop EC2.<br>&emsp;+ Cấu hình IAM Role và Amazon EventBridge Schedule.<br>&emsp;+ Kiểm tra hoạt động tự động của hệ thống. | **09/06/2026** | **09/06/2026** | https://000022.awsstudygroup.com/ |
| 4 | - **Workshop Manage Resources Using Tags and Resource Groups:**<br>&emsp;+ Gắn Tag cho các tài nguyên AWS.<br>&emsp;+ Tạo Resource Group theo Tag.<br>&emsp;+ Quản lý và tìm kiếm tài nguyên theo nhóm.<br>&emsp;+ Đánh giá lợi ích của Tag trong quản trị hệ thống. | **10/06/2026** | **10/06/2026** | https://000027.awsstudygroup.com/ |
| 5 | - Ôn tập các dịch vụ bảo mật và quản trị AWS.<br>&emsp;+ So sánh IAM, Cognito, IAM Identity Center và Organizations.<br>&emsp;+ Tổng hợp các phương pháp quản lý quyền truy cập và bảo vệ dữ liệu trên AWS.<br>&emsp;+ Phân tích vai trò của Security Hub trong hệ thống Cloud. | **11/06/2026** | **11/06/2026** | Tổng hợp tài liệu Workshop |
| 6 | - Thực hành tổng hợp.<br>&emsp;+ Kiểm tra hoạt động của AWS Security Hub.<br>&emsp;+ Kiểm tra Lambda tự động Start/Stop EC2 theo lịch.<br>&emsp;+ Quản lý tài nguyên bằng Resource Groups.<br>&emsp;+ Cleanup toàn bộ tài nguyên sau khi hoàn thành Workshop. | **12/06/2026** | **12/06/2026** | https://000018.awsstudygroup.com/<br>https://000022.awsstudygroup.com/<br>https://000027.awsstudygroup.com/ |

---

### Kết quả đạt được tuần 8:

* Hiểu được mô hình **Shared Responsibility Model**, từ đó phân biệt rõ trách nhiệm của AWS và khách hàng trong việc bảo vệ hạ tầng, hệ điều hành, dữ liệu và các dịch vụ đang sử dụng trên nền tảng Cloud.

* Nắm được chức năng của **AWS Identity and Access Management (IAM)**, **Amazon Cognito**, **AWS Organizations**, **IAM Identity Center (SSO)** và **AWS Key Management Service (KMS)**, đồng thời hiểu được vai trò của từng dịch vụ trong việc quản lý danh tính, phân quyền người dùng và mã hóa dữ liệu.

* Triển khai thành công **AWS Security Hub**, kích hoạt các tiêu chuẩn kiểm tra bảo mật, thu thập Security Findings và theo dõi tình trạng bảo mật của tài khoản AWS thông qua bảng điều khiển tập trung.

* Thực hành phân tích các cảnh báo bảo mật do Security Hub tổng hợp từ nhiều dịch vụ AWS, qua đó hiểu được cách phát hiện các cấu hình chưa an toàn và các khuyến nghị nhằm nâng cao mức độ bảo mật của hệ thống.

* Xây dựng thành công giải pháp tối ưu chi phí Amazon EC2 bằng **AWS Lambda**, cấu hình IAM Role và EventBridge để tự động khởi động hoặc dừng các EC2 Instance theo lịch, giúp giảm thời gian vận hành không cần thiết và tiết kiệm chi phí.

* Thực hiện gắn **Tags** cho các tài nguyên AWS và tạo **Resource Groups** để quản lý tài nguyên theo dự án, môi trường hoặc bộ phận, từ đó nâng cao khả năng tìm kiếm, theo dõi và quản trị hệ thống.

* Hiểu được vai trò của Tags trong việc hỗ trợ quản lý tài nguyên, kiểm soát chi phí, tự động hóa quy trình vận hành và tổ chức hạ tầng AWS một cách hiệu quả.

* Hoàn thành toàn bộ các bài thực hành về AWS Security Hub, AWS Lambda và Resource Groups, đồng thời thực hiện Cleanup toàn bộ tài nguyên sau khi kết thúc Workshop nhằm tránh phát sinh chi phí trên tài khoản AWS.