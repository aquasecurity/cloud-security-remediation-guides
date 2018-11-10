[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Root Account In Use

## Quick Info

| | |
|-|-|
| **Plugin Title** | Root Account In Use |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures the root account is not being actively used |
| **More Info** | The root account should not be used for day-to-day account management. IAM users, roles, and groups should be used instead. |
| **AWS Link** | http://docs.aws.amazon.com/general/latest/gr/root-vs-iam.html |
| **Recommended Action** | Create IAM users with appropriate group-level permissions for account access. Create an MFA token for the root account, and store its password and token generation QR codes in a secure place. |

## Detailed Remediation Steps

