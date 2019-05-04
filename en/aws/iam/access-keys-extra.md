[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Access Keys Extra

## Quick Info

| | |
|-|-|
| **Plugin Title** | Access Keys Extra |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Detects the use of more than one access key by any single user |
| **More Info** | Having more than one access key for a single user increases the chance of accidental exposure. Each account should only have one key that defines the users permissions. |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/ManagingCredentials.html |
| **Recommended Action** | Remove the extra access key for the specified user. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for IAM. </br> ![Step 2](/resources/aws/iam/access-keys-extra/step2.png "Step 2 - IAM")
