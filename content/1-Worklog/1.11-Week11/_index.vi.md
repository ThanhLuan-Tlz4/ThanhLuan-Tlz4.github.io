---
title: "Worklog Tuần 11"
date: 2024-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu tuần 11:

* Xây dựng hạ tầng Backend cho đồ án theo kiến trúc Serverless trên AWS.
* Triển khai cơ chế Upload tài liệu thông qua Amazon S3 Presigned URL.
* Xây dựng các REST API phục vụ quản lý tài liệu.
* Tích hợp các dịch vụ AWS phục vụ quá trình xử lý và phân tích tài liệu.
* Kiểm thử toàn bộ luồng Upload và quản lý tài liệu.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | --------------- |
| 2 | - Khởi tạo hạ tầng Backend.<br>&emsp;+ Tạo Amazon S3 Bucket lưu trữ tài liệu.<br>&emsp;+ Tạo Amazon DynamoDB Table và Global Secondary Index (GSI).<br>&emsp;+ Tạo IAM Role cho các AWS Lambda.<br>&emsp;+ Kiểm tra quyền truy cập giữa các dịch vụ. | **29/06/2026** | **29/06/2026** | AWS S3, DynamoDB, IAM Documentation |
| 3 | - Xây dựng chức năng Upload tài liệu.<br>&emsp;+ Tạo GenerateUploadUrl Lambda.<br>&emsp;+ Tạo API Gateway **POST /upload-url**.<br>&emsp;+ Kiểm thử tạo Presigned URL.<br>&emsp;+ Kiểm thử Upload (PUT) file trực tiếp lên Amazon S3 bằng Presigned URL. | **30/06/2026** | **30/06/2026** | AWS Lambda, API Gateway, Amazon S3 |
| 4 | - Xử lý sau khi Upload hoàn tất.<br>&emsp;+ Tạo UploadCompleted Lambda.<br>&emsp;+ Tạo S3 ObjectCreated Event Trigger.<br>&emsp;+ Cập nhật trạng thái tài liệu trong DynamoDB.<br>&emsp;+ Kiểm tra trạng thái **UPLOADED** sau khi Upload thành công. | **01/07/2026** | **01/07/2026** | AWS Lambda, Amazon S3 Event Notification |
| 5 | - Xây dựng các API quản lý tài liệu.<br>&emsp;+ Tạo GetDocument Lambda.<br>&emsp;+ Tạo ListDocuments Lambda.<br>&emsp;+ Tạo DeleteDocument Lambda.<br>&emsp;+ Tạo các API Route còn lại trên API Gateway.<br>&emsp;+ Kiểm thử các API CRUD. | **02/07/2026** | **02/07/2026** | AWS Lambda, API Gateway |
| 6 | - Hoàn thiện hệ thống Backend.<br>&emsp;+ Tạo DecisionEngine Lambda.<br>&emsp;+ Tích hợp Amazon Cognito JWT Authorizer.<br>&emsp;+ Kết nối Scan Orchestrator, Amazon GuardDuty và Amazon Bedrock.<br>&emsp;+ Bật Amazon CloudWatch Logging.<br>&emsp;+ Kiểm thử luồng chuyển tài liệu sang **Clean** hoặc **Reject**.<br>&emsp;+ Kiểm thử xử lý lỗi và hoàn thiện toàn bộ Backend. | **03/07/2026** | **03/07/2026** | AWS Lambda, Cognito, GuardDuty, Bedrock, CloudWatch |

---

### Kết quả đạt được tuần 11:

* Hoàn thành việc xây dựng hạ tầng Backend Serverless trên AWS, bao gồm Amazon S3, Amazon DynamoDB và IAM Role, tạo nền tảng cho quá trình phát triển hệ thống.

* Triển khai thành công cơ chế Upload tài liệu thông qua Amazon S3 Presigned URL, cho phép người dùng tải tệp trực tiếp lên Amazon S3 mà không cần truyền dữ liệu qua Backend, giúp giảm tải cho AWS Lambda và API Gateway.

* Xây dựng thành công API **POST /upload-url**, GenerateUploadUrl Lambda và kiểm tra đầy đủ quy trình tạo Presigned URL cũng như Upload tài liệu lên Amazon S3.

* Triển khai UploadCompleted Lambda kết hợp với Amazon S3 Event Notification để tự động cập nhật trạng thái tài liệu trong Amazon DynamoDB ngay sau khi Upload thành công.

* Hoàn thành các REST API phục vụ quản lý tài liệu gồm lấy thông tin tài liệu, danh sách tài liệu và xóa tài liệu, đồng thời kiểm thử thành công các chức năng CRUD thông qua Amazon API Gateway.

* Phát triển DecisionEngine Lambda nhằm xử lý luồng phân loại tài liệu, đồng thời tích hợp với Scan Orchestrator, Amazon GuardDuty và Amazon Bedrock để hỗ trợ quá trình phân tích và đánh giá tài liệu.

* Cấu hình Amazon Cognito JWT Authorizer giúp bảo vệ các API, chỉ cho phép người dùng đã xác thực truy cập vào hệ thống.

* Bật Amazon CloudWatch Logging để theo dõi quá trình thực thi của các AWS Lambda, hỗ trợ ghi nhận lỗi, kiểm tra log và phục vụ quá trình Debug.

* Kiểm thử thành công toàn bộ luồng xử lý từ tạo Presigned URL, Upload tài liệu, cập nhật trạng thái, quản lý tài liệu đến phân loại tài liệu, đảm bảo các thành phần Backend có thể phối hợp hoạt động ổn định theo kiến trúc Serverless đã thiết kế.