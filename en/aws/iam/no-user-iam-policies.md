[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / No User IAM Policies

## Quick Info

| | |
|-|-|
| **Plugin Title** | No User IAM Policies |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures IAM policies are not connected directly to IAM users |
| **More Info** | To reduce management complexity, IAM permissions should only be assigned to roles and groups. Users can then be added to those groups. Policies should not be applied directly to a user. |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#use-groups-for-permissions |
| **Recommended Action** | Create groups with the required policies, move the IAM users to the applicable groups, and then remove the inline and directly attached policies from the IAM user. |

## Detailed Remediation Steps

