[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Root Access Keys

## Quick Info

| | |
|-|-|
| **Plugin Title** | Root Access Keys |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures the root account is not using access keys |
| **More Info** | The root account should avoid using access keys. Since the root account has full permissions across the entire account, creating access keys for it only increases the chance that they are compromised. Instead, create IAM users with predefined roles. |
| **AWS Link** | http://docs.aws.amazon.com/general/latest/gr/managing-aws-access-keys.html |
| **Recommended Action** | Remove access keys for the root account and setup IAM users with limited permissions instead |

## Detailed Remediation Steps

