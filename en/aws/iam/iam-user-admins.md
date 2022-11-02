[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / IAM User Admins

## Quick Info

| | |
|-|-|
| **Plugin Title** | IAM User Admins |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures the number of IAM admins in the account are minimized |
| **More Info** | While at least two IAM admin users should be configured, the total number of admins should be kept to a minimum. |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started_create-admin-group.html |
| **Recommended Action** | Keep two users with admin permissions but ensure other IAM users have more limited permissions. |

## Detailed Remediation Steps

1. Log in to the AWS Management Console.
2. Select the "Services" option and search for IAM. </br> <img src="/resources/aws/iam/iam-user-admins/step2.png"/>
3. In the left navigation panel, select "Users" under "Access management".</br> <img src="/resources/aws/iam/iam-user-admins/step3.png"/>
4. Click on the User name of the IAM user that you want to inspect.</br> <img src="/resources/aws/iam/iam-user-admins/step4.png"/>
5. Scroll down and click the "Permissions" tab and check if the user has "AdministratorAccess" under Policy name then the user has administrator privileges.</br> <img src="/resources/aws/iam/iam-user-admins/step5.png"/>
6. Ensure that the user is authorised for administrative operations. If not then remove "AdministratorAccess" permission by clicking on the cross(x) on the extreme right column.</br> <img src="/resources/aws/iam/iam-user-admins/step6.png"/>
7. On the Detach Policy pop up click on "Detach" button to detach the AdministratorAccess policy from the user.</br> <img src="/resources/aws/iam/iam-user-admins/step7.png"/>
8. Repeat steps 4-7 for all other IAM users. There should be minimal number of users with AdministratorAccess policy.
