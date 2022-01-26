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
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for IAM. </br> <img src="/resources/aws/iam/access-keys-extra/step2.png"/>
3. Scroll down the left navigation panel and choose "Users" under "Access Management". </br><img src="/resources/aws/iam/access-keys-extra/step3.png"/>
4. Select the "User" that needs to be verified and click on the "User name" to access the selected "IAM User" and go to its configuration page.</br><img src="/resources/aws/iam/access-keys-extra/step4.png"/>
5. Under "Security Credentials" tab check the number of "Access Key ID". If there are more than "One Access Key ID" for the selected user than it increases the chance of accidental exposure.</br><img src="/resources/aws/iam/access-keys-extra/step5.png"/>
6. To remove the extra "Access Key" click on the cross(×) symbol at the extreme right to remove the selected key.</br> <img src="/resources/aws/iam/access-keys-extra/step6.png"/>
7. Click on "Deactivate" button in the delete confirmation popup box.</br><img src="/resources/aws/iam/access-keys-extra/step7.png"/>
8. Enter "Access key Id" in the text box and press the "Delete" button to delete the extra "Access Key".</br><img src="/resources/aws/iam/access-keys-extra/step8.png"/>
9. Repeat steps number 4 - 8 to check the "Access Keys" for all other IAM users.</br>
