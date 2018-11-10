[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / KMS / KMS Scheduled Deletion

## Quick Info

| | |
|-|-|
| **Plugin Title** | KMS Scheduled Deletion |
| **Cloud** | AWS |
| **Category** | KMS |
| **Description** | Detects KMS keys that are scheduled for deletion |
| **More Info** | Deleting a KMS key will permanently prevent all data encrypted using that key from being decrypted. Avoid deleting keys unless no encrypted data is in use. |
| **AWS Link** | http://docs.aws.amazon.com/kms/latest/developerguide/deleting-keys.html |
| **Recommended Action** | Disable the key deletion before the scheduled deletion time. |

## Detailed Remediation Steps

