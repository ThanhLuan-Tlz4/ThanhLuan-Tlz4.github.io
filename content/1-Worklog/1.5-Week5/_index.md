---

title: "Worklog Week 5"
date: 2024-01-01
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
----------------------

### Week 5 Objectives:

* Understand the Amazon S3 storage service and its basic components.
* Learn about data backup mechanisms with AWS Backup.
* Learn about Hybrid Storage architecture through AWS Storage Gateway.
* Practice creating Buckets, managing Objects, and deploying a Static Website on Amazon S3.
* Practice deploying a Backup Plan, restoring data, and connecting File Storage Gateway to an On-premises environment.

### Tasks to be implemented this week:

| Day | Tasks                                                                                                                                                                                                                                                                                                                | Start Date     | Completion Date | Reference Materials                                                                                         |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- | --------------- | ----------------------------------------------------------------------------------------------------------- |
| 2   | - Learn an overview of Amazon S3.<br>- Learn about Bucket, Object, Storage Class, and Versioning.<br>- Practice creating an S3 Bucket and uploading data.<br>- Become familiar with Amazon S3 security settings.                                                                                                     | **18/05/2026** | **18/05/2026**  | https://000057.awsstudygroup.com/                                                                           |
| 3   | - **Amazon S3 Workshop:**<br> + Manage Objects in an S3 Bucket.<br> + Configure Static Website Hosting.<br> + Practice Bucket Policy, Block Public Access, and Website Endpoint.<br> + Test Website accessibility from the Internet.                                                                                 | **19/05/2026** | **19/05/2026**  | https://000057.awsstudygroup.com/                                                                           |
| 4   | - **AWS Backup Workshop:**<br> + Deploy the infrastructure required for Backup.<br> + Create a Backup Vault and Backup Plan.<br> + Assign resources to be backed up.<br> + Perform data Backup and Restore.<br> + Verify the Restore process and clean up resources.                                                 | **20/05/2026** | **20/05/2026**  | https://000013.awsstudygroup.com/                                                                           |
| 5   | - **AWS Storage Gateway Workshop:**<br> + Prepare the Storage Gateway environment.<br> + Deploy File Storage Gateway on EC2.<br> + Create a File Share connected to Amazon S3.<br> + Configure SMB and mount the File Share from an On-premises machine.                                                             | **21/05/2026** | **21/05/2026**  | https://000024.awsstudygroup.com/                                                                           |
| 6   | - **Comprehensive Practice:**<br> + Test data synchronization between On-premises and Amazon S3 through File Storage Gateway.<br> + Evaluate the Backup and Restore process using AWS Backup.<br> + Compare data storage and protection methods on AWS.<br> + Clean up all resources after completing the Workshops. | **22/05/2026** | **22/05/2026**  | https://000013.awsstudygroup.com/<br>https://000024.awsstudygroup.com/<br>https://000057.awsstudygroup.com/ |

---

### Week 5 Achievements:

* Understood the Object Storage architecture of Amazon S3 and the relationship between Bucket, Object, Key, Storage Class, and Versioning in the process of managing data on AWS.

* Successfully deployed an Amazon S3 Bucket, uploaded, downloaded, and managed Objects through the AWS Management Console, while becoming familiar with data administration operations on S3.

* Successfully configured Static Website Hosting on Amazon S3 and set up a Bucket Policy and Website Endpoint to make website content publicly accessible, thereby understanding how static hosting services operate on AWS.

* Practiced configuring Block Public Access, Bucket Policy, and basic Amazon S3 security settings, thereby understanding how to control access permissions for stored data.

* Successfully deployed AWS Backup and created a Backup Vault, Backup Plan, and Resource Assignment to automatically back up AWS resources according to a schedule, while understanding the mechanisms for managing and automating data backups.

* Successfully performed resource Backup and Restore through AWS Backup, checked Recovery Points, and verified data recovery capability, thereby understanding the process of data protection and disaster recovery.

* Deployed File Storage Gateway on Amazon EC2, created a File Share linked to Amazon S3, and configured the SMB protocol to provide shared storage for an On-premises environment.

* Mounted the File Share from an On-premises machine and tested data synchronization between the local system and Amazon S3, thereby understanding the Hybrid Storage mechanism and how AWS Storage Gateway connects traditional infrastructure with Cloud storage services.

* Evaluated the roles of Amazon S3, AWS Backup, and AWS Storage Gateway in building storage, backup, and data synchronization systems on AWS, while also completing the cleanup of all resources after the hands-on exercises to avoid unexpected costs.
