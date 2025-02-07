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
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for IAM. </br><img src="/resources/aws/iam/no-user-iam-policies/step2.png"/>
3. Scroll down the left navigation panel and select "Users" under "Access management".</br><img src="/resources/aws/iam/no-user-iam-policies/step3.png"/>
4. Click on the IAM User name that you want to inspect.</br><img src="/resources/aws/iam/no-user-iam-policies/step4.png"/>
5. Scroll down on the IAM user configuration page and click on the "Permissions" tab.</br><img src="/resources/aws/iam/no-user-iam-policies/step5.png"/>
6. Ensure that there are no policies "Attached directly". </br><img src="/resources/aws/iam/no-user-iam-policies/step6.png"/>
7. If there are any policies "Attached directly" then they should be removed and assigned through either a group or role.</br><img src="/resources/aws/iam/no-user-iam-policies/step7.png"/>
8. Repeat steps 4 – 7 for all IAM users.
