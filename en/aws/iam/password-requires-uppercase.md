[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Password Requires Uppercase

## Quick Info

| | |
|-|-|
| **Plugin Title** | Password Requires Uppercase |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures password policy requires at least one uppercase letter |
| **More Info** | A strong password policy enforces minimum length, expirations, reuse, and symbol usage |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/Using_ManagingPasswordPolicies.html |
| **Recommended Action** | Update the password policy to require the use of uppercase letters |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for IAM. </br><img src="/resources/aws/iam/password-requires-uppercase/step2.png"/>
3. Scroll down the left navigation panel and choose "Account Settings" under "Access management". </br><img src="/resources/aws/iam/password-requires-uppercase/step3.png"/>
4. Under the "Password Policy" configuration panel scroll down and click on "Change password policy" button.</br><img src="/resources/aws/iam/password-requires-uppercase/step4.png"/>
5. On the Set password policy page scroll down and check the "Require at least one uppercase letter from Latin alphabet (A-Z)". If the checkbox is not selected than the password policy does not  enforces the use of uppercase letters in password.</br><img src="/resources/aws/iam/password-requires-uppercase/step5.png"/>
6. Click on the checkbox next to "Require at least one uppercase letter from Latin alphabet (A-Z)" so "Password Policy" requires at least one uppercase letter to make the password more strong and secure. </br> <img src="/resources/aws/iam/password-requires-uppercase/step6.png"/>
7. Click on the "Save changes" button to make the necessary changes.</br><img src="/resources/aws/iam/password-requires-uppercase/step7.png"/>
8. Now "Password Policy" ensures that the password requires uppercase letters.</br>
