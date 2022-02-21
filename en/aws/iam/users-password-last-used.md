[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Users Password Last Used

## Quick Info

| | |
|-|-|
| **Plugin Title** | Users Password Last Used |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Detects users with password logins that have not been used for a period of time and that should be decommissioned |
| **More Info** | Having numerous, unused user accounts extends the attack surface. If users do not log into their accounts for more than the defined period of time, the account should be deleted. |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_passwords_admin-change-user.html |
| **Recommended Action** | Delete old user accounts that allow password-based logins and have not been used recently. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for IAM. </br> <img src="/resources/aws/iam/users-password-last-used/step2.png"/>
3. Scroll down the left navigation panel and choose "Credential report". Click on the "Download Report" button to download a report that lists all your account's users and the status of their various credentials. </br><img src="/resources/aws/iam/users-password-last-used/step3.png"/>
4. Open the downloaded credentials report and check the "password_last_used_date" column for the root account. If the timestamp value is recorded within the last 7 days the above credentials have been used to access the AWS account.</br><img src="/resources/aws/iam/users-password-last-used/step3.png"/>


6. Scroll down the left navigation panel and choose "Users". 
7. Select the "User" that needs to be verified and click on the "User name" to access the selected "IAM User".</br><img src="/resources/aws/iam/users-password-last-used/step4.png"/>
8. Click on the "Security Credentials" under the configuration page.</br><img src="/resources/aws/iam/users-password-last-used/step5.png"/>
9. Scroll down the "Security Credentials" tab and check the "Console password".Check the "Console password" section for "last signed in". If "last signed in" is showing for the period more than 180 days than the password is not been used for a period of time.</br><img src="/resources/aws/iam/users-password-last-used/step6.png"/>
10. Repeat steps number 2 - 6 to verify for other IAM users.</br>
11. Go to the "Users" page and select the "User" whose password is not been used for a period of time now. </br><img src="/resources/aws/iam/users-password-last-used/step8.png"/>
12. Click on the "Delete user" button at the top to delete the selected user. </br><img src="/resources/aws/iam/users-password-last-used/step9.png"/>
13. On the "Delete user" tab click on the "Yes, delete" button to delete the selected IAM user. </br><img src="/resources/aws/iam/users-password-last-used/step10.png"/>
14. Repeat steps number 8 - 10 to delete the other IAM users whose passwords are not used for a period of time. </br>
