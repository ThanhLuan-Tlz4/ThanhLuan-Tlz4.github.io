---
title : "User Authentication"
date : 2024-01-01
weight : 2
chapter : false
pre : " <b> 5.2 </b> "
---

#### Authentication and Authorization with Amazon Cognito

In this section, you will configure **Amazon Cognito User Pool** to manage user accounts, authenticate users, and issue **JWT Tokens** for the application. You will also create an **App Client**, configure the managed login page, create the **Users** and **Admins** groups, and test the login flow before integrating authentication with the Frontend and Amazon API Gateway.

The user's group information is stored in the `cognito:groups` claim of the JWT Token. This allows the system to distinguish between regular users and administrators when they access protected APIs.


#### Content

- [Create Amazon Cognito User Pool](5.2.1-create-user-pool/)
- [Create User Groups](5.2.2-create-groups/)