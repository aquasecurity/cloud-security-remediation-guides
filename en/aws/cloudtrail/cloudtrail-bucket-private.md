[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudTrail / CloudTrail Bucket Private

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudTrail Bucket Private |
| **Cloud** | AWS |
| **Category** | CloudTrail |
| **Description** | Ensures CloudTrail logging bucket is not publicly accessible |
| **More Info** | CloudTrail buckets contain large amounts of sensitive account data and should only be accessible by logged in users. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonS3/latest/dev/example-bucket-policies.html |
| **Recommended Action** | Set the S3 bucket access policy for all CloudTrail buckets to only allow known users to access its files. |

## Detailed Remediation Steps

