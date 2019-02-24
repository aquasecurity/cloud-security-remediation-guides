[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / KMS / KMS Key Policy

## Quick Info

| | |
|-|-|
| **Plugin Title** | KMS Key Policy |
| **Cloud** | AWS |
| **Category** | KMS |
| **Description** | Validates the KMS key policy to ensure least-privilege access. |
| **More Info** | KMS key policies should be designed to limit the number of users who can perform encrypt and decrypt operations. Each application should use its own key to avoid over exposure. |
| **AWS Link** | http://docs.aws.amazon.com/kms/latest/developerguide/key-policies.html |
| **Recommended Action** | Modify the KMS key policy to remove any wildcards and limit the number of users and roles that can perform encrypt and decrypt operations using the key. |

## Detailed Remediation Steps

