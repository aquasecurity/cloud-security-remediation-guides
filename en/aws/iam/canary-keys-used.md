[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Canary Keys Used

## Quick Info

| | |
|-|-|
| **Plugin Title** | Canary Keys Used |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Detects when a special canary-token access key has been used |
| **More Info** | Canary access keys can be created with limited permissions and then used to detect when a potential breach occurs. |
| **AWS Link** | https://docs.aws.amazon.com/IAM/latest/UserGuide/ManagingCredentials.html |
| **Recommended Action** | Create a canary access token and provide its user to CloudSploit. If CloudSploit detects that the account is in use, it will trigger a failure. |

## Detailed Remediation Steps

