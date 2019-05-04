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
2. Select the "Services" option and search for IAM. </br> ![Step 2](/resources/aws/iam/access-keys-last-used/step2.png "Step 2 - IAM")
3. Scroll down the left navigation panel and choose "Users". </br>![Step 3](/resources/aws/iam/access-keys-last-used/step3.png "Step 3 - Users")
4. Select the "User" that needs to be verified and click on the "User name" to access the selected "IAM User".</br>![Step 4](/resources/aws/iam/access-keys-last-used/step4.png "Step 4 - User name")
5. Click on the "Security Credentials" under the configuration page.</br>![Step 5](/resources/aws/iam/access-keys-last-used/step5.png "Step 5 - Security Credentials")
6. Scroll down and under "Security Credentials" check the "Last used" cloumn in "Access keys" to determine the last date of "Access Key" used by the selected "User".</br>![Step 6](/resources/aws/iam/access-keys-extra/step6.png "Step 6 - Access Key ID")
7. Repeat the steps number 4 - 6 to check the "Access Keys" last used date for another user.</br>
8. To remove the "Access Key" which is not used for a period of time click on "Security Credentials" under IAM user configuration page and select the "Access Key ID" which needs to be removed.</br> ![Step 8](/resources/aws/iam/access-keys-extra/step8.png "Step 8 - Access Key")
9. Click on the cross(×) symbol at the extreme right to remove the selected key. </br> ![Step 9](/resources/aws/iam/access-keys-extra/step9.png "Step 6 - Delete")
10. Click on "Delete" button under "Delete access key" tab to delete the extra "Access Key".</br>![Step 10](/resources/aws/iam/access-keys-extra/step10.png "Step 10 - Delete")

