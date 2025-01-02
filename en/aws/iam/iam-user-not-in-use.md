[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / IAM User Account Not In Use

## Quick Info

| | |
|-|-|
| **Plugin Title** | IAM User Account Not In Use |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensure that IAM user accounts are being actively used. |
| **More Info** | To increase the security of your AWS account, remove IAM user accounts that have not been used over a certain period of time. |
| **AWS Link** | https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_finding-unused.html |
| **Recommended Action** | Delete IAM user accounts which are not being actively used or change the password or deactivate the access keys so they no longer have access. |

## Detailed Remediation Steps

1. Log in to the AWS Management Console.
2. Select Services and search for IAM.  
    <img src="/resources/aws/iam/iam-policies-present/step1.png"/>
3. In the IAM dashboard, click on Users from the left navigation panel.  
    <img src="/resources/aws/iam/iam-policies-present/step2.png"/>
4. For each user, go to the Access Advisor tab to review the last accessed date and identify accounts that have not been used recently.
5. For inactive accounts, choose to either delete the user or disable their access by removing passwords and deactivating access keys.  
    <img src="/resources/aws/iam/iam-policies-present/step3.png"/>
6. Confirm changes to disable access for each inactive user. Repeat for other IAM accounts as necessary.