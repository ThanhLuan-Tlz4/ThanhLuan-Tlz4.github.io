---

title: "Workshop"
date: 2024-01-01
weight: 5
chapter: false
pre: " <b> 5. </b> "
--------------------

# Secure AI-Driven Document Platform

In this workshop, you will build a serverless platform on AWS that allows documents to be uploaded, scanned for malware, analyzed with AI, and released only when they meet security policies.

The solution combines synchronous APIs with an event-driven processing workflow. Users and administrators interact through a React application; the backend uses managed services including Amazon Cognito, Amazon API Gateway, AWS Lambda, Amazon S3, Amazon DynamoDB, Amazon SQS, Amazon EventBridge, Amazon GuardDuty Malware Protection, Amazon Bedrock Mantle, Amazon CloudFront, and Amazon CloudWatch.
## The System You Will Build

After completing the workshop, the platform will include:

* Login with Cognito for regular users and administrators.
* User APIs and administrator APIs protected by JWT.
* Direct browser upload to S3 through short-lived Presigned URLs.
* Separate storage areas for quarantined, safe, and rejected documents.
* Automatic malware scanning using GuardDuty Malware Protection for S3.
* AI analysis to detect phishing, fraud, social engineering, credential theft, and prompt injection risks.
* A Decision Engine that determines the final result from malware results, AI results, and administrator reviews.
* APIs that allow users to list, view, download, and delete documents.
* An administration workflow to review documents, manage documents, and manage users.
* A React frontend hosted privately in S3 and distributed through CloudFront with HTTPS.
* End-to-end testing, operational logs, and a complete cleanup process.

## Architecture Overview

![Secure AI-Driven Document Platform Architecture](/images/5-Workshop/5.1-Workshop-overview/secure-document-platform-architecture.png)

| Layer             | AWS Services                                     | Responsibility                                                  |
| ----------------- | ------------------------------------------------ | --------------------------------------------------------------- |
| User access       | CloudFront, Amazon S3, Amazon Cognito            | Distribute the web application and authenticate users           |
| API               | Amazon API Gateway, AWS Lambda                   | Authorize requests and process user and administrator functions |
| Document storage  | Amazon S3                                        | Isolate newly uploaded, approved, and rejected documents        |
| Orchestration     | Amazon SQS, Amazon EventBridge, DynamoDB Streams | Connect processing stages without tight coupling                |
| Security analysis | GuardDuty Malware Protection, Bedrock Mantle     | Detect malware and analyze content risk                         |
| State             | Amazon DynamoDB                                  | Store owner, status, scan results, AI results, and decisions    |
| Operations        | Amazon CloudWatch                                | Store logs, support troubleshooting, and verify the system      |

## Document Processing Flow

1. The user logs in through Amazon Cognito and receives a token for the web session.
2. The Frontend calls the protected upload API using the Cognito access token.
3. The upload Lambda creates a `documentId`, writes the initial record to DynamoDB, and returns a short-lived S3 Presigned URL.
4. The browser uploads the document directly to the `uploads/` prefix of the quarantine bucket.
5. Amazon S3 sends the upload event to Amazon SQS, while GuardDuty Malware Protection scans the new object.
6. The GuardDuty result is routed through Amazon EventBridge to the Lambda function that processes scan results. The Lambda function normalizes the result and updates DynamoDB.
7. Only documents without malware are extracted into text and analyzed for content using AI through Bedrock Mantle.
8. DynamoDB Streams triggers the Decision Engine when malware results, AI results, or administrator reviews are available.
9. Safe documents are copied to the clean bucket; blocked documents are copied to the rejected bucket. The source object is deleted only after the destination copy has been verified.
10. The Frontend reads the current status through the Document API. Documents requiring human review remain in the `MANUAL_REVIEW` status until an authorized administrator submits a decision.

Documents confirmed to contain malware are always rejected and cannot have their results overridden by AI or administrators.

## Workshop Roadmap

Complete the sections in order because each section uses resources created in previous sections.

| Section                                         | Content                                                                                  |
| ----------------------------------------------- | ---------------------------------------------------------------------------------------- |
| [5.1 Workshop Overview](5.1-workshop-overview/) | Learn about the problem, architecture, objectives, and expected results                  |
| [5.2 Authentication](5.2-authentication/)       | Create a Cognito user pool, app client, group, and test accounts                         |
| [5.3 Storage](5.3-storage/)                     | Create S3 buckets, a DynamoDB table, prefixes, and CORS configuration                    |
| [5.4 Document Upload](5.4-upload/)              | Build the Lambda function and API for creating Presigned URLs, then test document upload |
| [5.5 Malware Scan](5.5-malware-scan/)           | Configure SQS, S3 events, GuardDuty, and scan result processing                          |
| [5.6 AI Analysis](5.6-ai-analysis/)             | Prepare extraction libraries, configure Mantle, and analyze safe documents               |
| [5.7 Decision](5.7-decision/)                   | Create the Decision Engine and move documents to the clean or rejected area              |
| [5.8 Document API](5.8-document-api/)           | Add APIs for listing, viewing, deleting, downloading, and retrieving scan results        |
| [5.9 Administration](5.9-admin/)                | Add document review and user management features with authorization                      |
| [5.10 Frontend](5.10-frontend/)                 | Build the Vite application and deploy it through S3 and CloudFront                       |
| [5.11 Testing](5.11-testing/)                   | Test security, processing branches, retry behavior, and browser behavior                 |
| [5.12 Cleanup](5.12-cleanup/)                   | Safely delete workshop resources and verify that no billable resources remain            |

## Security Principles Throughout the Workshop

* The browser never receives the application’s AWS access key or secret key.
* API Gateway authenticates JWT; Lambda checks document ownership and Admin permissions on the server side.
* Presigned URLs are short-lived and allow only the correct S3 operation on the correct object key.
* Newly uploaded documents must remain in the quarantine area until all mandatory checks are completed.
* Content extracted from documents is treated as untrusted data; AI only classifies it and does not follow instructions inside the document.
* DynamoDB conditional updates and idempotent handlers protect the system from duplicate events and competing decisions.
* The Decision Engine verifies the destination copy before deleting the source object in the quarantine area.
* Logs contain only identifiers and state transitions; they do not record tokens, secrets, full document content, or Presigned URLs.

## Preparation Before Starting

You need to prepare:

* An AWS account or workshop sandbox with permissions to create the services used in this document.
* Access to the AWS Management Console and a terminal configured with AWS CLI for command-line steps.
* A local development environment to create Lambda packages and the Vite frontend.
* A modern browser to test Cognito, APIs, upload functionality, and CloudFront.
* Sample TXT, PDF, and DOCX files that do not contain sensitive information. Only use harmless anti-malware test files guided in the malware scan section; never use real malware.

Unless a section provides different instructions, deploy the main workload in `ap-southeast-1`. Always check the Region displayed in each step, especially when configuring Bedrock Mantle credentials and global services such as CloudFront and IAM.

Record generated values such as bucket names, API URLs, Cognito IDs, Lambda names, and the CloudFront domain. Later sections will continue using these values.

## Completion Criteria

The workshop is complete when you can demonstrate that:

* Regular users can log in, upload safe documents, track status, and download only after the final decision is `SAFE`.
* Documents with malware or high risk are rejected and cannot be downloaded.
* Users cannot view, delete, or download documents belonging to other users.
* Administrators can review appropriate documents but cannot override a result confirmed to contain malware.
* Duplicate events and simultaneous decisions do not create conflicting metadata or multiple effective document copies.
* The application works through CloudFront HTTPS while the S3 bucket containing the frontend remains private.
* CloudWatch Logs allow each test to be traced without exposing credentials or sensitive content.
* All workshop resources are deleted after final verification.

Select **5.1 Workshop Overview** to begin.
