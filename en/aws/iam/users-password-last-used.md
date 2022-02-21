[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Users Password Last Used

## Quick Info

| | |
|-|-|
| **Plugin Title** | Users Password Last Used |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Detects users with password logins that have not been used for a period of time and that should be decommissioned |
| **More Info** | Having numerous, unused user accounts extends the attack surface. If users do not log into their accounts for more than the defined period of time, the account should either be deleted or have console login disabled. |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_passwords_admin-change-user.html |
| **Recommended Action** | Delete old user accounts that allow password-based logins and have not been used recently. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for IAM. </br> <img src="/resources/aws/iam/users-password-last-used/step2.png"/>
3. Scroll down the left navigation panel and choose "Credential report". Click on the "Download Report" button to download a report that lists all your account's users and the status of their various credentials. </br><img src="/resources/aws/iam/users-password-last-used/step3.png"/>
4. Open the downloaded credentials report and check the "password_last_used_date" column for each IAM account. If the timestamp value for "password_last_used_date" is recorded within the last 7 days, the above credentials have been used to access the AWS account. If however, the timestamp value is older than 90 days, then the account should be deleted or disabled.</br><img src="/resources/aws/iam/users-password-last-used/step4.png"/>
5. Scroll down the left navigation panel and choose "Users". </br><img src="/resources/aws/iam/users-password-last-used/step5.png"/>
6. Select the "User" that needs to be verified and click on the "User name" to access the selected IAM User.</br><img src="/resources/aws/iam/users-password-last-used/step6.png"/>
7. Click on the "Security Credentials" tab under the configuration page.</br><img src="/resources/aws/iam/users-password-last-used/step7.png"/>
8. Under the "Security Credentials" tab check the "Console password" section for status "Enabled/Disabled". If the status is "Enabled" then the console sign in is enabled and needs to be disabled. </br><img src="/resources/aws/iam/users-password-last-used/step8.png"/>
9. Click on "Manage" to open "Manage console acess" pop up. </br><img src="/resources/aws/iam/users-password-last-used/step9.png"/>
10. Select "Disable" for the Console access and click on "Apply" button. </br><img src="/resources/aws/iam/users-password-last-used/step10.png"/>
11. Repeat steps number 2 - 11 to verify for other IAM users.</br>
