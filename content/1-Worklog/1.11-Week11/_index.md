---

title: "Worklog Week 11"
date: 2024-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
-----------------------

### Week 11 Objectives:

* Build the Backend infrastructure for the project using a Serverless architecture on AWS.
* Implement the document Upload mechanism through Amazon S3 Presigned URLs.
* Build REST APIs for document management.
* Integrate AWS services to support document processing and analysis.
* Test the entire document Upload and management flow.

### Tasks to be implemented this week:

| Day | Tasks                                                                                                                                                                                                                                                                                                                                                            | Start Date     | Completion Date | Reference Materials                                 |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- | --------------- | --------------------------------------------------- |
| 2   | - Initialize the Backend infrastructure.<br> + Create an Amazon S3 Bucket for document storage.<br> + Create an Amazon DynamoDB Table and Global Secondary Index (GSI).<br> + Create IAM Roles for AWS Lambda functions.<br> + Verify access permissions between services.                                                                                       | **29/06/2026** | **29/06/2026**  | AWS S3, DynamoDB, IAM Documentation                 |
| 3   | - Build the document Upload functionality.<br> + Create the GenerateUploadUrl Lambda.<br> + Create the API Gateway **POST /upload-url** endpoint.<br> + Test Presigned URL generation.<br> + Test direct file Upload (PUT) to Amazon S3 using the Presigned URL.                                                                                                 | **30/06/2026** | **30/06/2026**  | AWS Lambda, API Gateway, Amazon S3                  |
| 4   | - Process the document after the Upload is completed.<br> + Create the UploadCompleted Lambda.<br> + Create an S3 ObjectCreated Event Trigger.<br> + Update the document status in DynamoDB.<br> + Verify the **UPLOADED** status after a successful Upload.                                                                                                     | **01/07/2026** | **01/07/2026**  | AWS Lambda, Amazon S3 Event Notification            |
| 5   | - Build document management APIs.<br> + Create the GetDocument Lambda.<br> + Create the ListDocuments Lambda.<br> + Create the DeleteDocument Lambda.<br> + Create the remaining API Routes in API Gateway.<br> + Test the CRUD APIs.                                                                                                                            | **02/07/2026** | **02/07/2026**  | AWS Lambda, API Gateway                             |
| 6   | - Complete the Backend system.<br> + Create the DecisionEngine Lambda.<br> + Integrate the Amazon Cognito JWT Authorizer.<br> + Connect the Scan Orchestrator, Amazon GuardDuty, and Amazon Bedrock.<br> + Enable Amazon CloudWatch Logging.<br> + Test the document flow to **Clean** or **Reject**.<br> + Test error handling and complete the entire Backend. | **03/07/2026** | **03/07/2026**  | AWS Lambda, Cognito, GuardDuty, Bedrock, CloudWatch |

---

### Week 11 Achievements:

* Completed the Serverless Backend infrastructure on AWS, including Amazon S3, Amazon DynamoDB, and IAM Roles, creating the foundation for system development.

* Successfully implemented the document Upload mechanism through Amazon S3 Presigned URLs, allowing users to upload files directly to Amazon S3 without sending the data through the Backend, thereby reducing the load on AWS Lambda and API Gateway.

* Successfully built the **POST /upload-url** API and the GenerateUploadUrl Lambda, and fully tested the process of generating a Presigned URL and uploading documents to Amazon S3.

* Deployed the UploadCompleted Lambda together with Amazon S3 Event Notification to automatically update the document status in Amazon DynamoDB immediately after a successful Upload.

* Completed the REST APIs for document management, including retrieving document information, listing documents, and deleting documents, while successfully testing the CRUD functions through Amazon API Gateway.

* Developed the DecisionEngine Lambda to process the document classification flow and integrated it with the Scan Orchestrator, Amazon GuardDuty, and Amazon Bedrock to support document analysis and evaluation.

* Configured the Amazon Cognito JWT Authorizer to protect the APIs and allow only authenticated users to access the system.

* Enabled Amazon CloudWatch Logging to monitor AWS Lambda execution, record errors, inspect logs, and support the Debugging process.

* Successfully tested the entire processing flow, from generating the Presigned URL and uploading the document to updating its status, managing documents, and classifying documents, ensuring that the Backend components could work together reliably according to the designed Serverless architecture.
