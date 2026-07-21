---
title : "Configure Amazon S3 CORS"
date : 2024-01-01
weight : 4
chapter : false
pre : " <b> 5.3.4 </b> "
---

CORS allows the frontend running on localhost or through CloudFront to upload documents directly to Amazon S3 using Presigned URLs.

## Configure CORS for the Quarantine bucket

1. Open the [Amazon S3 console](https://console.aws.amazon.com/s3/).
2. Select the bucket:

```text
securedocs-quarantine-<account-id>
```

3. Open the **Permissions** tab.
4. Scroll to **Cross-origin resource sharing (CORS)**.
5. Choose **Edit**.

![Open S3 CORS configuration](/images/5-Workshop/5.3/5.3.4/5.3.4.1.png)

6. Enter the following JSON configuration:

```json
[
  {
    "AllowedHeaders": [
      "*"
    ],
    "AllowedMethods": [
      "PUT",
      "GET",
      "HEAD"
    ],
    "AllowedOrigins": [
      "http://localhost:5173",
      "https://YOUR-CLOUDFRONT-DOMAIN.cloudfront.net"
    ],
    "ExposeHeaders": [
      "ETag"
    ],
    "MaxAgeSeconds": 3000
  }
]
```

7. Replace `YOUR-CLOUDFRONT-DOMAIN` with your project's CloudFront domain.
8. Choose **Save changes**.

## Configure CORS for the Clean bucket

Perform this step only if the frontend needs to download or preview documents directly from the Clean bucket.

```json
[
  {
    "AllowedHeaders": [
      "*"
    ],
    "AllowedMethods": [
      "GET",
      "HEAD"
    ],
    "AllowedOrigins": [
      "http://localhost:5173",
      "https://YOUR-CLOUDFRONT-DOMAIN.cloudfront.net"
    ],
    "ExposeHeaders": [
      "ETag",
      "Content-Type"
    ],
    "MaxAgeSeconds": 3000
  }
]
```

{{% notice warning %}}
Do not use `*` for **AllowedOrigins** in the production environment. Allow only the localhost domain during development and the official CloudFront domain of the project.
{{% /notice %}}

{{% notice note %}}
CORS does not make the bucket public. Access permissions are still controlled by IAM, bucket policies, and Presigned URLs.
{{% /notice %}}