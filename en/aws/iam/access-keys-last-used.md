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
1. Log into the AWS Management Console.
2. Select the "Services" option and search for IAM. </br> <img src="/resources/aws/iam/access-keys-last-used/step2.png"/>
3. Scroll down the left navigation panel and choose "Users". </br><img src="/resources/aws/iam/access-keys-last-used/step3.png"/>
4. Select the "User" that needs to be verified and click on the "User name" to access the selected "IAM User".</br><img src="/resources/aws/iam/access-keys-last-used/step4.png"/>
5. Click on the "Security Credentials" under the configuration page.</br><img src="/resources/aws/iam/access-keys-last-used/step5.png"/>
6. Scroll down and under "Security Credentials" check the "Last used" cloumn in "Access keys" to determine the last date of "Access Key" used by the selected "User".</br><img src="/resources/aws/iam/access-keys-last-used/step6.png"/>
7. Repeat the steps number 4 - 6 to check the "Access Keys" last used date for another user.</br>
8. To remove the "Access Key" which is not used for a period of time click on "Security Credentials" under IAM user configuration page and select the "Access Key ID" which needs to be removed.</br> <img src="/resources/aws/iam/access-keys-last-used/step8.png"/>
9. Click on the cross(×) symbol at the extreme right to remove the selected key. </br> <img src="/resources/aws/iam/access-keys-last-used/step9.png"/>
10. Click on "Delete" button under "Delete access key" tab to delete the extra "Access Key".</br><img src="/resources/aws/iam/access-keys-last-used/step10.png"/>
