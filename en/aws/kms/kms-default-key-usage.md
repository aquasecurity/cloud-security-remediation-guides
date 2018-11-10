[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / KMS / KMS Default Key Usage

## Quick Info

| | |
|-|-|
| **Plugin Title** | KMS Default Key Usage |
| **Cloud** | AWS |
| **Category** | KMS |
| **Description** | Checks AWS services to ensure the default KMS key is not being used |
| **More Info** | It is recommended not to use the default key to avoid encrypting disparate sets of data with the same key. Each application should have its own customer-managed KMS key |
| **AWS Link** | http://docs.aws.amazon.com/kms/latest/developerguide/concepts.html |
| **Recommended Action** | Avoid using the default KMS key |

## Detailed Remediation Steps

