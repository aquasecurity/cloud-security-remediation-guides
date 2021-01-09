[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / RDS / RDS CMK Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | RDS CMK Encryption |
| **Cloud** | AWS |
| **Category** | RDS |
| **Description** | Ensures RDS instances are encrypted with KMS Customer Master Keys(CMKs). |
| **More Info** | RDS instances should be encrypted with Customer Master Keys in order to have full control over data encryption and decryption. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Overview.Encryption.html |
| **Recommended Action** | RDS does not currently allow modifications to encryption after the instance has been launched, so a new instance will need to be created with KMS CMK encryption enabled. |

## Detailed Remediation Steps




