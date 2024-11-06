[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / IAM User Without Permissions
## Quick Info

| | |
|-|-|
| **Plugin Title** | IAM User Without Permissions |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | IAM users are created to perform any Console, CLI or API based operations on AWS cloud accounts. They are associated with policies that grant them permissions to perform required operations. An IAM user without any permission is a security risk, it is recommended to either add required permissions or delete them to adhere to compliance standards. |
| **More Info** | Ensure that no IAM user exists without any permissions. |
| **AWS Link** | https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html |
| **Recommended Action** | Modify IAM user and attach new permissions or delete the user. |

## Detailed Remediation Steps

1. Log in to the AWS Management Console.
2. Select Services and search for IAM.  
   <img src="/resources/aws/iam/iam-user-without-permissions/step1.png"/>
3. In the IAM dashboard, click on Users from the left navigation panel.  
   <img src="/resources/aws/iam/iam-user-without-permissions/step2.png"/>
4. Select a user from the list and go to the Permissions tab to review any attached policies.
5. If no policies are attached, either click on Add permissions to assign appropriate permissions or consider deleting the user if no access is needed.  
   <img src="/resources/aws/iam/iam-user-without-permissions/step3.png"/>
6. Repeat these steps for other IAM users to ensure all users have the required permissions or are removed if unnecessary.