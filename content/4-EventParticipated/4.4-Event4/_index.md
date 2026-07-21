---

title: "Event 4"
date: 2026-07-11
weight: 4
chapter: false
pre: " <b> 4.4. </b> "
----------------------

# Reflection Report on the “First Cloud Journey & Community Day” Event - Part 2

### Purpose of the Event

* Provide a roadmap and study strategy for the AWS Cloud Practitioner certification exam.
* Change the mindset about system monitoring and Service Level Agreements (SLA) from the perspective of user experience.
* Introduce an AI-powered solution for automated security testing (Pentest) and vulnerability assessment with AWS Security Agent.

### List of Speakers

* **Ngô Lê Tấn Huy** - Speaker on the topic Inside The Exam: AWS Cloud Practitioner.
* **Nguyễn Huỳnh Sơn** - Freshly graduated from HUFLIT / Ex Infrastructure Reliability Engineer at SPS, presented about SLA and Monitoring.
* **Thịnh Nguyễn** - DevOps/DevSecOps/Cloud Engineer at Styl Solutions, presented about AWS Security Agent.

### Highlighted Content

#### Strategy for Conquering AWS Cloud Practitioner (CLF-C02)

* **Exam structure:** Requires an overall mindset about digital transformation rather than deep technical configuration. The exam focuses most heavily on Cloud Technology and Services (34%) and Security and Compliance (30%).
* **Security responsibility (Shared Responsibility Model):** AWS protects "Security OF the Cloud" (infrastructure), while customers are responsible for "Security IN the Cloud" (data, IAM configuration).
* **Exam tips:** Use the elimination technique (immediately eliminate “made-up” services), avoid overcomplicating the problem, and learn through keywords (for example: "Decouple/Microservices" is associated with SQS).

#### SLA and System Monitoring Mindset

* **The gap between "healthy infrastructure" and "happy users":** A dashboard showing green CPU and RAM metrics (stable) does not necessarily mean that users can successfully log in or complete payments.
* **Monitoring Pyramid:** Monitoring needs to be established across multiple layers, from Cloud Provider, Infrastructure, and Application to Business and Customer Experience.
* **Incident response process:** Apply a risk management loop from Identify -> Monitor with Metrics/Logs -> Alert through CloudWatch/SNS -> Improve the process. Dr. Werner Vogels once said: *"Everything fails all the time, so plan for failure and nothing fails"*.

#### Security Automation with AWS Security Agent (Frontier Agent)

* **Problems with traditional Pentest:** It is time-consuming, expensive (possibly reaching 5k - 20k USD), and highly dependent on the individual skills of the tester.
* **The power of Autonomous Reasoning:** Powered by Amazon Bedrock, the AI agent is capable of automatically reading architecture documents, reviewing source code (Code Security) on Pull Requests, and performing real attacks (Active Penetration Testing) to validate vulnerabilities instead of only chatting like a normal LLM.
* **Limitations to note:** The current agent will be blocked by security layers such as MFA, biometrics, or mTLS. At the same time, it has difficulty detecting vulnerabilities related to deep business logic.

### What Was Learned

#### Design & System Thinking

* System quality assessment must start from Business Metrics and the actual customer experience instead of focusing only on technical server metrics.
* There is a strong shift in the cybersecurity industry, where AI is no longer used only to detect anomalies but can now automatically chain attack scenarios (exploit chains) to perform penetration testing like a real hacker.

#### Technical Architecture

* Understood how to set up an automated alerting flow: from measuring failed metrics (for example: Login Failure), setting thresholds on CloudWatch Alarm, pushing notifications through SNS Topic, and alerting the team through Slack/Email.
* Understood the basic difference between protecting web applications with a firewall (AWS WAF) and proactively hunting for vulnerabilities with AI (AWS Security Agent).

### Application to Work

* **Strengthening the internship profile:** Plan to practice on AWS Free Tier and set a goal to obtain the AWS Cloud Practitioner certification to strengthen the Cloud Computing foundation, serving as a perfect stepping stone for upcoming Network Engineer or IT Support internship positions.
* **Upgrading network security projects:** Integrate the user experience monitoring mindset (SLA/Monitoring) into current research projects on monitoring systems and log analysis. When configuring alerts on tools such as Wazuh or Falco, it is necessary to classify which alerts directly affect end users.
* **DevSecOps in the development process:** Research the application of automated source code review tools or simulations of AWS Security Agent in personal software projects to check for basic vulnerabilities (such as SQL Injection) before merging code.

### Experience During the Event

* The event provided extremely practical and fresh perspectives. Realizing that "green infrastructure does not mean users are fine" was a valuable lesson that completely changed the way maintenance and network operations are viewed.
* The demo of an AI agent performing automated pentesting was especially engaging, showing that the automation trend in the cybersecurity industry is developing very quickly and requires continuous technology updates to avoid falling behind.

### Photos from the Event

![image](/images/events/event_4.png)
