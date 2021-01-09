[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / S3 / S3 Bucket Encryption In Transit

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 Bucket Encryption In Transit |
| **Cloud** | AWS |
| **Category** | S3 |
| **Description** | Ensures S3 buckets have bucket policy statements that deny insecure transport |
| **More Info** | S3 bucket policies can be configured to deny access to the bucket over HTTP. |
| **AWS Link** | https://aws.amazon.com/premiumsupport/knowledge-center/s3-bucket-policy-for-config-rule/ |
| **Recommended Action** | Add statements to the bucket policy that deny all S3 actions when SecureTransport is false. Resources must be list of bucket ARN and bucket ARN with wildcard. |

## Detailed Remediation Steps




