---
title: "Event 4"
date: 2026-07-11
weight: 4
chapter: false
pre: " <b> 4.4. </b> "
---

# Bài thu hoạch sự kiện “First Cloud Journey & Community Day” - Phần 2

### Mục Đích Của Sự Kiện

- Cung cấp lộ trình và chiến lược ôn thi chứng chỉ AWS Cloud Practitioner.
- Thay đổi tư duy về giám sát hệ thống (Monitoring) và cam kết chất lượng dịch vụ (SLA) từ góc nhìn trải nghiệm người dùng.
- Giới thiệu giải pháp tự động hóa kiểm thử bảo mật (Pentest) và rà soát lỗ hổng bằng AI với AWS Security Agent.

### Danh Sách Diễn Giả

- **Ngô Lê Tấn Huy** - Diễn giả chủ đề Inside The Exam: AWS Cloud Practitioner.
- **Nguyễn Huỳnh Sơn** - Freshly graduated from HUFLIT / Ex Infrastructure Reliability Engineer tại SPS, trình bày về SLA and Monitoring.
- **Thịnh Nguyễn** - DevOps/DevSecOps/Cloud Engineer tại Styl Solutions, trình bày về AWS Security Agent.

### Nội Dung Nổi Bật

#### Chiến lược chinh phục AWS Cloud Practitioner (CLF-C02)
- **Cấu trúc bài thi:** Đòi hỏi tư duy tổng quan về chuyển đổi số hơn là cấu hình kỹ thuật sâu. Tập trung nhiều nhất vào Cloud Technology and Services (34%) và Security and Compliance (30%).
- **Trách nhiệm bảo mật (Shared Responsibility Model):** AWS bảo vệ "Security OF the Cloud" (hạ tầng), khách hàng chịu trách nhiệm "Security IN the Cloud" (dữ liệu, cấu hình IAM).
- **Mẹo làm bài thi:** Sử dụng kỹ thuật loại trừ (loại bỏ ngay các dịch vụ "được bịa ra"), không nghĩ quá phức tạp hóa vấn đề, và kết hợp học qua từ khóa (ví dụ: "Decouple/Microservices" đi liền với SQS). 

#### SLA và Tư duy Giám sát hệ thống (Monitoring)
- **Khoảng cách giữa "Hạ tầng khỏe" và "Người dùng vui":** Một bảng điều khiển (dashboard) hiển thị CPU và RAM đều xanh (ổn định) không đồng nghĩa với việc người dùng có thể đăng nhập hay thanh toán thành công.
- **Tháp giám sát (Monitoring Pyramid):** Cần thiết lập giám sát ở nhiều tầng, từ Cloud Provider, Infrastructure, Application cho đến Business và Customer Experience.
- **Quy trình xử lý sự cố:** Áp dụng vòng lặp quản lý rủi ro từ Nhận dạng (Identify) -> Giám sát bằng Metric/Log -> Cảnh báo qua CloudWatch/SNS -> Cải thiện quy trình. Dr. Werner Vogels từng nói: *"Everything fails all the time, so plan for failure and nothing fails"*.

#### Tự động hóa bảo mật với AWS Security Agent (Frontier Agent)
- **Vấn đề của Pentest truyền thống:** Tốn thời gian, đắt đỏ (có thể lên tới 5k - 20k USD) và phụ thuộc nhiều vào kỹ năng cá nhân của người thực hiện.
- **Sức mạnh của Autonomous Reasoning:** Được trợ lực bởi Amazon Bedrock, tác tử AI có khả năng tự động đọc tài liệu kiến trúc, rà soát mã nguồn (Code Security) trên Pull Request và thực hiện tấn công thực tế (Active Penetration Testing) để xác thực lỗ hổng thay vì chỉ chat như LLM thông thường.
- **Hạn chế cần lưu ý:** Tác tử hiện tại sẽ bị chặn đứng bởi các lớp bảo mật như MFA, Sinh trắc học, hoặc mTLS. Đồng thời, nó gặp khó khăn trong việc phát hiện các lỗ hổng liên quan đến logic nghiệp vụ sâu.

### Những Gì Học Được

#### Tư Duy Thiết Kế & Hệ Thống
- Đánh giá chất lượng hệ thống phải bắt nguồn từ các chỉ số kinh doanh (Business Metrics) và trải nghiệm thực tế của khách hàng thay vì chỉ tập trung vào các chỉ số kỹ thuật của máy chủ.
- Sự chuyển dịch mạnh mẽ trong ngành an toàn thông tin khi AI không chỉ dùng để phát hiện bất thường mà đã có thể tự động xâu chuỗi các kịch bản tấn công (exploit chains) để kiểm thử xâm nhập như một hacker thực thụ.

#### Kiến Trúc Kỹ Thuật
- Nắm được cách thiết lập luồng cảnh báo tự động: từ việc đo lường số liệu bị lỗi (ví dụ: Login Failure), đặt ngưỡng trên CloudWatch Alarm, đẩy thông báo qua SNS Topic và báo động đến Slack/Email của đội ngũ.
- Hiểu được sự khác biệt cơ bản giữa việc bảo vệ ứng dụng web bằng tường lửa (AWS WAF) với việc chủ động săn tìm lỗ hổng bằng AI (AWS Security Agent).

### Ứng Dụng Vào Công Việc

- **Củng cố hồ sơ thực tập:** Lên kế hoạch thực hành trên AWS Free Tier và đặt mục tiêu thi lấy chứng chỉ AWS Cloud Practitioner để củng cố nền tảng điện toán đám mây, làm bước đệm hoàn hảo cho các vị trí thực tập Network Engineer hoặc IT Support sắp tới.
- **Nâng cấp dự án bảo mật mạng:** Tích hợp tư duy giám sát trải nghiệm người dùng (SLA/Monitoring) vào các dự án nghiên cứu hệ thống giám sát và phân tích log hiện tại. Khi cấu hình cảnh báo trên các công cụ như Wazuh hay Falco, cần chú ý phân loại cảnh báo nào ảnh hưởng trực tiếp đến người dùng cuối.
- **DevSecOps trong quy trình phát triển:** Nghiên cứu áp dụng các công cụ rà soát mã nguồn tự động hoặc mô phỏng AWS Security Agent vào các dự án phần mềm cá nhân để kiểm tra các lỗ hổng cơ bản (như SQL Injection) trước khi merge code.

### Trải nghiệm trong event

- Sự kiện mang lại những góc nhìn cực kỳ thực tế và mới mẻ. Việc nhận ra "hạ tầng xanh không có nghĩa là người dùng đang ổn" là một bài học đắt giá, làm thay đổi hoàn toàn cách nhìn nhận về việc bảo trì và vận hành mạng.
- Phần demo ứng dụng tác tử AI thực hiện pentest tự động đặc biệt cuốn hút, cho thấy xu hướng tự động hóa trong ngành An toàn thông tin mạng đang diễn ra rất nhanh, đòi hỏi bản thân phải liên tục cập nhật công nghệ để không bị bỏ lại phía sau.

### Hình ảnh trong sử kiện

![image](/images/events/event_4.png)
