---

title: "Worklog Week 2"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
----------------------

### Week 2 Objectives:

* Understand identity and access management mechanisms on AWS through AWS Identity and Access Management (IAM).
* Understand how IAM User, Group, Role, and Policy work.
* Practice using AWS CLI to manage AWS resources.
* Apply the Least Privilege principle to build a secure AWS environment.
* Complete hands-on exercises on IAM and AWS CLI in the First Cloud AI Journey program.

### Tasks to be implemented this week:

| Day | Tasks                                                                                                                                                                                                                                              | Start Date     | Completion Date | Reference Materials                          |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- | --------------- | -------------------------------------------- |
| 2   | - Learn about AWS Identity and Access Management (IAM).<br>- Concepts of Authentication and Authorization.<br>- Root User and IAM User.<br>- Shared Responsibility Model.                                                                          | **27/04/2026** | **27/04/2026**  | https://000002.awsstudygroup.com/            |
| 3   | - Learn about IAM User, IAM Group, Managed Policy, and Inline Policy.<br>- **Practice:**<br> + Create an IAM User.<br> + Create an IAM Group.<br> + Attach Policies to Users and Groups.<br> + Test access permissions.                            | **28/04/2026** | **28/04/2026**  | https://000002.awsstudygroup.com/2-iam-user/ |
| 4   | - Learn about IAM Role and AWS STS.<br>- **Practice:**<br> + Create an IAM Role for Amazon EC2.<br> + Attach the Role to an EC2 Instance.<br> + Test access to Amazon S3 through the IAM Role.                                                     | **29/04/2026** | **29/04/2026**  | https://000002.awsstudygroup.com/3-iam-role/ |
| 5   | - Learn about AWS CLI and authentication using IAM Credentials.<br>- **Practice:**<br> + aws configure.<br> + aws sts get-caller-identity.<br> + aws iam list-users.<br> + aws ec2 describe-instances.<br> + aws s3 ls.                            | **30/04/2026** | **30/04/2026**  | https://000010.awsstudygroup.com/            |
| 6   | - **Comprehensive Practice:**<br> + Build a complete IAM model including User, Group, Role, and Policy.<br> + Manage resources using both AWS Management Console and AWS CLI.<br> + Verify permissions according to the Least Privilege principle. | **01/05/2026** | **02/05/2026**  | https://000002.awsstudygroup.com/            |

---

### Week 2 Achievements:

* Understood the AWS identity and access management model through AWS Identity and Access Management (IAM).

* Understood the functions and usage of:

  * IAM User.
  * IAM Group.
  * IAM Role.
  * Managed Policy.
  * Inline Policy.

* Understood and applied the **Least Privilege** principle when granting permissions to users and services.

* Successfully practiced creating and managing multiple IAM Users, IAM Groups, and IAM Roles for system administration scenarios.

* Understood the temporary authentication mechanism through IAM Role and AWS Security Token Service (STS).

* Used AWS CLI to perform basic administrative operations such as:

  * Checking AWS account information.
  * Listing IAM Users.
  * Checking EC2 Instances.
  * Listing S3 Buckets.
  * Verifying the current user information using `aws sts get-caller-identity`.

* Developed the ability to combine AWS Management Console and AWS CLI to manage AWS resources effectively.

* Built a basic permission model according to AWS security principles, creating a foundation for hands-on exercises on Amazon VPC and Networking in the following weeks.
