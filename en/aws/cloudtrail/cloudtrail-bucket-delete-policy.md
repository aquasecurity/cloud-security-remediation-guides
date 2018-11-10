[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudTrail / CloudTrail Bucket Delete Policy

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudTrail Bucket Delete Policy |
| **Cloud** | AWS |
| **Category** | CloudTrail |
| **Description** | Ensures CloudTrail logging bucket has a policy to prevent deletion of logs without an MFA token |
| **More Info** | To provide additional security, CloudTrail logging buckets should require an MFA token to delete objects |
| **AWS Link** | http://docs.aws.amazon.com/AmazonS3/latest/dev/Versioning.html#MultiFactorAuthenticationDelete |
| **Recommended Action** | Enable MFA delete on the CloudTrail bucket |

## Detailed Remediation Steps

