[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / SSH Keys Rotated

## Quick Info

| | |
|-|-|
| **Plugin Title** | SSH Keys Rotated |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures SSH keys are not older than 180 days in order to reduce accidental exposures |
| **More Info** | SSH keys should be rotated frequently to avoid having them accidentally exposed. |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_ssh-keys.html |
| **Recommended Action** | To rotate an SSH key, first create a new public-private key pair, then upload the public key to AWS and delete the old key. |

## Detailed Remediation Steps

