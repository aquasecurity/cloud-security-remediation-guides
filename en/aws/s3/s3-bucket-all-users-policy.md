[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / S3 / S3 Bucket All Users Policy

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 Bucket All Users Policy |
| **Cloud** | AWS |
| **Category** | S3 |
| **Description** | Ensures S3 bucket policies do not allow global write, delete, or read permissions |
| **More Info** | S3 buckets can be configured to allow the global principal to access the bucket via the bucket policy. This policy should be restricted only to known users or accounts. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonS3/latest/dev/using-iam-policies.html |
| **Recommended Action** | Remove wildcard principals from the bucket policy statements. |

## Detailed Remediation Steps

