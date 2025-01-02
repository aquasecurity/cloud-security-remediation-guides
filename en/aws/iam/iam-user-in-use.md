[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / IAM User Account In Use

## Quick Info

| | |
|-|-|
| **Plugin Title** | IAM User Account In Use |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensure that IAM user accounts are not being actively used. |
| **More Info** | IAM users, roles, and groups should not be used for day-to-day account management. |
| **AWS Link** | https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_create.html |
| **Recommended Action** | Delete IAM user accounts which are being actively used. |

## Detailed Remediation Steps

1. Log in to the AWS Management Console.
2. Select Services and search for IAM.  
    <img src="/resources/aws/iam/iam-user-not-in-use/step1.png"/>
3. In the IAM dashboard, click on Users from the left navigation panel.  
    <img src="/resources/aws/iam/iam-user-not-in-use/step2.png"/>
4. Review each user’s Access Advisor tab to check for recent activity and determine if the user account is actively in use.
5. For actively used accounts, consider disabling or deleting the IAM user account to prevent non-role-based management.
6. If deletion is needed, select the user, click Delete user, and confirm the action. Repeat for other actively used IAM accounts.  
    <img src="/resources/aws/iam/iam-user-not-in-use/step3.png"/>