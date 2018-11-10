[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / S3 / S3 Bucket All Users ACL

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 Bucket All Users ACL |
| **Cloud** | AWS |
| **Category** | S3 |
| **Description** | Ensures S3 buckets do not allow global write, delete, or read ACL permissions |
| **More Info** | S3 buckets can be configured to allow anyone, regardless of whether they are an AWS user or not, to write objects to a bucket or delete objects. This option should not be configured unless their is a strong business requirement. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonS3/latest/UG/EditingBucketPermissions.html |
| **Recommended Action** | Disable global all users policies on all S3 buckets and ensure both the bucket ACL is configured with least privileges. |

## Detailed Remediation Steps

