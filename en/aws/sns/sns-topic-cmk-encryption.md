[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / SNS / SNS Topic CMK Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | SNS Topic CMK Encryption |
| **Cloud** | AWS |
| **Category** | SNS |
| **Description** | Ensures Amazon SNS topics are encrypted with KMS Customer Master Keys (CMKs). |
| **More Info** | AWS SNS topics should be  encrypted with KMS Customer Master Keys (CMKs) instead of AWS managed-keysin order to have a more granular control over the SNS data-at-rest encryption and decryption process. |
| **AWS Link** | https://docs.aws.amazon.com/sns/latest/dg/sns-server-side-encryption.html |
| **Recommended Action** | Update SNS topics to use Customer Master Keys (CMKs) for Server-Side Encryption. |

## Detailed Remediation Steps




