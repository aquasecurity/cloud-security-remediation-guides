[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudFront / Public S3 CloudFront Origin

## Quick Info

| | |
|-|-|
| **Plugin Title** | Public S3 CloudFront Origin |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Detects the use of an S3 bucket as a CloudFront origin without an origin access identity |
| **More Info** | When S3 is used as an origin for a CloudFront bucket, the contents should be kept private and an origin access identity should allow CloudFront access. This prevents someone from bypassing the caching benefits that CloudFront provides, repeatedly loading objects directly from S3, and amassing a large access bill. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/private-content-restricting-access-to-s3.html |
| **Recommended Action** | Create an origin access identity for CloudFront, then make the contents of the S3 bucket private. |

## Detailed Remediation Steps

