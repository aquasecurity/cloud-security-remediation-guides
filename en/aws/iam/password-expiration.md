[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Password Expiration

## Quick Info

| | |
|-|-|
| **Plugin Title** | Password Expiration |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures password policy enforces a strong password expiration configuration |
| **More Info** | A strong password policy enforces minimum length, expirations, reuse, and symbol usage |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/Using_ManagingPasswordPolicies.html |
| **Recommended Action** | Enable a strong password expiration policy for the account |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for IAM. </br><img src="/resources/aws/iam/password-expiration/step2.png"/>
3. Scroll down the left navigation panel and choose "Account Settings" under "Access management". </br><img src="/resources/aws/iam/password-expiration/step3.png"/>
4. Under the "Password Policy" configuration panel scroll down and click on "Change password policy" button.</br><img src="/resources/aws/iam/password-expiration/step4.png"/>
5. On the Set password policy page scroll down and check the "Enable password expiration". If the "Enable password expiration" checkbox is not ticked then the password won't expire in any number of days. </br><img src="/resources/aws/iam/password-expiration/step5.png"/>
6. Click on the "Enable password expiration" checkbox and mention the days under "Expire passwords in (days)" so that the password will expire after the specified days. For better security reasons define the number of days to at least more than 90. Click on "Allow users to change their own password" as well.</br><img src="/resources/aws/iam/password-expiration/step6.png"/>
7. Click on the "Save changes" button to make the necessary changes.</br><img src="/resources/aws/iam/password-expiration/step7.png"/>
8. Now "Password Policy" will enforce a password expiration for all the IAM users.</br>
