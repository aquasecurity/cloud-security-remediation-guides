[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / IAM User Present

## Quick Info

| | |
|-|-|
| **Plugin Title** | IAM User Present |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensure that at least one IAM user exists so that access to your AWS services and resources is made only through IAM users instead of the root account. |
| **More Info** | To protect your AWS root account and adhere to IAM security best practices, create individual IAM users to access your AWS environment. |
| **AWS Link** | https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html |
| **Recommended Action** | Create IAM user(s) and use them to access AWS services and resources. |

## Detailed Remediation Steps

1. Log in to the AWS Management Console.
2. Select Services and search for IAM.  
   <img src="/resources/aws/iam/iam-user-present/step1.png"/>
3. In the IAM dashboard, click on Users from the left navigation panel.  
   <img src="/resources/aws/iam/iam-user-present/step2.png"/>
4. Click on Add user to create a new IAM user.
5. Enter a user name and configure the access type, choosing either programmatic access or AWS Management Console access as required.
6. Follow the prompts to assign permissions, set up tags, and review the settings before creating the user.
7. Complete the creation and provide the new IAM user with access details. Repeat if additional users are needed.