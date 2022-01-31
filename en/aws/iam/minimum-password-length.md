[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Minimum Password Length

## Quick Info

| | |
|-|-|
| **Plugin Title** | Minimum Password Length |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures password policy requires a password of at least a minimum number of characters |
| **More Info** | A strong password policy enforces minimum length, expirations, reuse, and symbol usage |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/Using_ManagingPasswordPolicies.html |
| **Recommended Action** | Increase the minimum length requirement for the password policy |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for IAM. </br><img src="/resources/aws/iam/minimum-password-length/step2.png"/>
3. Scroll down the left navigation panel and choose "Account Settings" under "Access management". </br><img src="/resources/aws/iam/minimum-password-length/step3.png"/>
4. Under the "Password Policy" configuration panel scroll down and click on "Change password policy" button.</br><img src="/resources/aws/iam/minimum-password-length/step4.png"/>
5. On the Set password policy page scroll down and check the "Enforce minimum password length". If the password length is set less than 8 characters than the password security is at risk. </br><img src="/resources/aws/iam/minimum-password-length/step5.png"/>
6. Mention the minimum characters required to 14 in the textbox. Click the checkbox against "Require at least one uppercase letter" and "Require at least one lowercase letter" to make the password more secure. </br><img src="/resources/aws/iam/minimum-password-length/step6.png"/>
7. Click on the "Save changes" button to make the necessary changes.</br><img src="/resources/aws/iam/minimum-password-length/step7.png"/>
8. Now "Password Policy" requires at least 14 characters with one uppercase and one lowercase character for a strong and secure password.</br>

