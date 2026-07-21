---

title: "Worklog Week 9"
date: 2024-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
----------------------

### Week 9 Objectives:

* Reinforce knowledge of security and access management services on AWS.
* Understand how to control access to EC2 resources through IAM Policies combined with Resource Tags.
* Learn how to limit the permissions of IAM Users and IAM Roles using IAM Permission Boundaries.
* Practice encrypting data at rest using AWS Key Management Service (AWS KMS).
* Improve the ability to design security systems according to the Least Privilege principle on AWS.

### Tasks to be implemented this week:

| Day | Tasks                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | Start Date     | Completion Date | Reference Materials                                                                                                                |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------- | --------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| 2   | - Study the theory of the **Shared Responsibility Model**, **IAM**, **Amazon Cognito**, **AWS Organizations**, **IAM Identity Center (SSO)**, and **AWS KMS** to reinforce AWS security knowledge.<br>- **Manage Access to EC2 Services with Resource Tags through IAM Services Workshop:**<br> + Learn about access control mechanisms using Resource Tags.<br> + Create an IAM Policy using Tag conditions.<br> + Test EC2 access permissions for different resource groups. | **15/06/2026** | **15/06/2026**  | https://www.youtube.com/watch?v=tsobAlSg19g&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=150<br>https://000028.awsstudygroup.com/ |
| 3   | - **Limitation of User Rights with IAM Permission Boundary Workshop:**<br> + Learn how Permission Boundaries work.<br> + Create an IAM Policy Boundary.<br> + Apply a Permission Boundary to an IAM User and IAM Role.<br> + Test access permission limits after configuration.                                                                                                                                                                                                | **16/06/2026** | **16/06/2026**  | https://000030.awsstudygroup.com/                                                                                                  |
| 4   | - **Encrypt at Rest with AWS KMS Workshop:**<br> + Create a Customer Managed Key (CMK).<br> + Configure data encryption using AWS KMS.<br> + Test permissions for using the KMS Key.<br> + Practice encrypting storage resources on AWS.                                                                                                                                                                                                                                       | **17/06/2026** | **17/06/2026**  | https://000033.awsstudygroup.com/                                                                                                  |
| 5   | - Summarize knowledge of IAM and AWS KMS.<br> + Compare IAM Policy, Resource Tags, and Permission Boundary.<br> + Analyze permission models based on the Least Privilege principle.<br> + Evaluate the role of AWS KMS in protecting data on the Cloud.                                                                                                                                                                                                                        | **18/06/2026** | **18/06/2026**  | Workshop materials compilation                                                                                                     |
| 6   | - Comprehensive practice.<br> + Test EC2 access permissions based on Resource Tags.<br> + Verify the effectiveness of the Permission Boundary.<br> + Confirm that data is encrypted using AWS KMS.<br> + Clean up all resources after completing the Workshop.                                                                                                                                                                                                                 | **19/06/2026** | **19/06/2026**  | https://000028.awsstudygroup.com/<br>https://000030.awsstudygroup.com/<br>https://000033.awsstudygroup.com/                        |

---

### Week 9 Achievements:

* Reinforced knowledge of AWS security services and understood the relationship between IAM, Resource Tags, Permission Boundaries, and AWS KMS in building access control and data protection systems.

* Successfully practiced managing access to Amazon EC2 through **IAM Policies combined with Resource Tags**, creating policies that use `Condition` statements to allow users to operate only on EC2 Instances with matching Tags.

* Tested and verified the access permissions of multiple IAM Users for resources with different Tags, thereby understanding how to implement access control models by project or department without creating multiple separate IAM Policies.

* Successfully deployed an **IAM Permission Boundary**, created a Permission Boundary Policy, and applied it to an IAM User or IAM Role to limit the maximum scope of permissions that could be granted to these identities.

* Tested scenarios in which granted permissions exceeded the Permission Boundary, thereby understanding how the Permission Boundary acts as an additional control layer to prevent permissions from being granted beyond the allowed scope.

* Successfully created a **Customer Managed Key (CMK)** using AWS Key Management Service (AWS KMS), managed encryption key usage permissions, and practiced encrypting data at rest across AWS services.

* Understood the **Encrypt at Rest** mechanism on AWS and learned how AWS KMS securely manages encryption keys and performs data encryption and decryption while maintaining access control.

* Evaluated the effectiveness of combining Resource Tags, IAM Policies, Permission Boundaries, and AWS KMS to build a security system based on the **Least Privilege** principle, strengthening access control and data protection on the AWS platform.

* Completed all hands-on exercises and cleaned up resources after finishing the Workshop to ensure that the AWS environment did not incur unexpected costs.
