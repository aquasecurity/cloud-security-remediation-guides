[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / KMS / KMS Key Rotation

## Quick Info

| | |
|-|-|
| **Plugin Title** | KMS Key Rotation |
| **Cloud** | AWS |
| **Category** | KMS |
| **Description** | Ensures KMS keys are set to rotate on a regular schedule |
| **More Info** | All KMS keys should have key rotation enabled. AWS will handle the rotation of the encryption key itself, as well as storage of previous keys, so previous data does not need to be re-encrypted before the rotation occurs. |
| **AWS Link** | http://docs.aws.amazon.com/kms/latest/developerguide/rotate-keys.html |
| **Recommended Action** | Enable yearly rotation for the KMS key |

## Detailed Remediation Steps

