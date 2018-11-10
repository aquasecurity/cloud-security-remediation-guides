[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Access Keys Rotated

## Quick Info

| | |
|-|-|
| **Plugin Title** | Access Keys Rotated |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures access keys are not older than 180 days in order to reduce accidental exposures |
| **More Info** | Access keys should be rotated frequently to avoid having them accidentally exposed. |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/ManagingCredentials.html |
| **Recommended Action** | To rotate an access key, first create a new key, replace the key and secret throughout your app or scripts, then set the previous key to disabled. Once you ensure that no services are broken, then fully delete the old key. |

## Detailed Remediation Steps

