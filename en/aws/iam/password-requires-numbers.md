[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Password Requires Numbers

## Quick Info

| | |
|-|-|
| **Plugin Title** | Password Requires Numbers |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures password policy requires the use of numbers |
| **More Info** | A strong password policy enforces minimum length, expirations, reuse, and symbol usage |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/Using_ManagingPasswordPolicies.html |
| **Recommended Action** | Update the password policy to require the use of numbers |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for IAM. </br><img src="/resources/aws/iam/password-requires-numbers/step2.png"/>
3. Scroll down the left navigation panel and choose "Account Settings". </br><img src="/resources/aws/iam/password-requires-numbers/step3.png"/>
4. Under the "Password Policy" configuration panel scroll down and check the "Require at least one number". If the checkbox is not selected than the password policy does not enforces the use of numbers in password.</br><img src="/resources/aws/iam/password-requires-numbers/step4.png"/>
5. Repeat steps number 3 and 4 to ensures password policy requires numbers.</br>
6. Click on the checkbox next to "Require at least one number" so "Password Policy" requires at least one number to make the password more strong and secure. </br> <img src="/resources/aws/iam/password-requires-numbers/step6.png"/>
7. Click on the "Apply Password Policy" button to make the necessary changes.</br><img src="/resources/aws/iam/password-requires-numbers/step7.png"/>
