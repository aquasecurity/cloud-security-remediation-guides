[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Users Password And Keys

## Quick Info

| | |
|-|-|
| **Plugin Title** | Users Password And Keys |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Detects whether users with a console password are also using access keys |
| **More Info** | Access keys should only be assigned to machine users and should not be used for accounts that have console password access. |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/ManagingCredentials.html |
| **Recommended Action** | Remove access keys from all users with console access. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for IAM. </br> <img src="/resources/aws/iam/users-password-and-keys/step2.png"/>
3. Scroll down the left navigation panel and choose "Users". </br><img src="/resources/aws/iam/users-password-and-keys/step3.png"/>
4. On the "Users" page, click on the "User" in the "User name" column.</br> <img src="/resources/aws/iam/users-password-and-keys/step4.png"/>
5. In the "Users - Summary" page, click on the Security Credentials to check whether the selected user have Console access and Access Keys as well.</br> <img src="/resources/aws/iam/users-password-and-keys/step5.png"/>
6. Repeat steps number 2 - 5 to check other users in the account.</br>
7. Navigate to IAM dashboard at https://console.aws.amazon.com/iam/.</br>
8. In the "IAM dashboard", click on the "Users" option at the left navigation panel and select the user who have Access key and Console access both.</br> <img src="/resources/aws/iam/users-password-and-keys/step8.png"/>
9. In the "users - Summary" page, click on the Security Credentials to remove the "Access key" from the selected user.</br> <img src="/resources/aws/iam/users-password-and-keys/step9.png"/>
10. In the "Security Credential" page, scroll down and click on the (x) button under the Access Keys to remove the access key.</br> <img src="/resources/aws/iam/users-password-and-keys/step10.png"/>
11. On the "Delete" tab, first click on "Deactivate" the key and then provide the Key Attribute and click on the "Delete" button.</br> <img src="/resources/aws/iam/users-password-and-keys/step11.png"/>
12. Repeat steps number 7 - 11 to remove access keys from all users with console access. </br>
