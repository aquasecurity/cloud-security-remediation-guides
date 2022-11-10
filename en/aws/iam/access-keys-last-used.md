[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Access Keys Last Used

## Quick Info

| | |
|-|-|
| **Plugin Title** | Access Keys Last Used |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Detects access keys that have not been used for a period of time and that should be decommissioned |
| **More Info** | Having numerous, unused access keys extends the attack surface. Access keys should be removed if they are no longer being used. |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/ManagingCredentials.html |
| **Recommended Action** | Log into the IAM portal and remove the offending access key. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for IAM. </br> <img src="/resources/aws/iam/access-keys-last-used/step2.png"/>
3. Scroll down the left navigation panel and choose "Users" under "Access Management". </br><img src="/resources/aws/iam/access-keys-last-used/step3.png"/>
4. Select the "User" that needs to be verified and click on the "User name" to access the selected "IAM User" and go to its configuration page.</br><img src="/resources/aws/iam/access-keys-last-used/step4.png"/>
5. Under "Security Credentials" tab check the "Last used" column in "Access keys" to determine the last date of "Access Key" used by the selected "User".</br><img src="/resources/aws/iam/access-keys-last-used/step5.png"/>
6. To remove the "Access Key" which is not used for a period of time click on the cross(×) symbol at the extreme right to remove the selected key. </br> <img src="/resources/aws/iam/access-keys-last-used/step6.png"/>
7. Click on "Deactivate" button in the delete confirmation popup box.</br><img src="/resources/aws/iam/access-keys-last-used/step7.png"/>
8. Enter "Access key Id" in the text box and press the "Delete" button to delete the last used "Access Key".</br><img src="/resources/aws/iam/access-keys-last-used/step8.png"/>
9. Repeat steps number 4 - 8 to check the "Access Keys" for all other IAM users.
