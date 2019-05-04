[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Access Keys Extra

## Quick Info

| | |
|-|-|
| **Plugin Title** | Access Keys Extra |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Detects the use of more than one access key by any single user |
| **More Info** | Having more than one access key for a single user increases the chance of accidental exposure. Each account should only have one key that defines the users permissions. |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/ManagingCredentials.html |
| **Recommended Action** | Remove the extra access key for the specified user. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for IAM. </br> <img src="/resources/aws/iam/access-keys-extra/step2.png"/>
3. Scroll down the left navigation panel and choose "Users". </br><img src="/resources/aws/iam/access-keys-extra/step3.png"/>
4. Select the "User" that needs to be verified and click on the "User name" to access the selected "IAM User".</br><img src="/resources/aws/iam/access-keys-extra/step4.png"/>
5. Click on the "Security Credentials" under the configuration page.</br><img src="/resources/aws/iam/access-keys-extra/step5.png"/>
6. Scroll down and under "Security Credentials" check the number of "Access Key ID". If there are more than "One Access Key ID" for the selected user than it increases the chance of accidental exposure.</br><img src="/resources/aws/iam/access-keys-extra/step6.png"/>
7. Repeat the steps number 4 - 6 to check the "Access Keys" for another user.</br>
8. To remove the extra "Access Key" click on "Security Credentials" under IAM user configuration page and select the "Access Key ID" which needs to be removed.</br> <img src="/resources/aws/iam/access-keys-extra/step8.png"/>
9. Click on the cross(×) symbol at the extreme right to remove the selected key. </br> <img src="/resources/aws/iam/access-keys-extra/step9.png"/>
10. Click on "Delete" button under "Delete access key" tab to delete the extra "Access Key".</br><img src="/resources/aws/iam/access-keys-extra/step10.png"/>
