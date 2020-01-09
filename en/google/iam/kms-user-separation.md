[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / IAM / KMS User Separation

## Quick Info

| | |
|-|-|
| **Plugin Title** | KMS User Separation |
| **Cloud** | GOOGLE |
| **Category** | IAM |
| **Description** | Ensures that no users have the KMS admin role and any one of the CryptoKey roles. |
| **More Info** | Ensuring that no users have the KMS admin role and any one of the CryptoKey roles follows separation of duties, where no user should have access to resources out of the scope of duty. |
| **GOOGLE Link** | https://cloud.google.com/iam/docs/overview |
| **Recommended Action** | Ensure that no service accounts have both the KMS admin role and any of CryptoKey roles attached. |

## Detailed Remediation Steps


