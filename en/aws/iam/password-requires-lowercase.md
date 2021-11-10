[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Password Requires Lowercase

## Quick Info

| | |
|-|-|
| **Plugin Title** | Password Requires Lowercase |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures password policy requires at least one lowercase letter |
| **More Info** | A strong password policy enforces minimum length, expirations, reuse, and symbol usage |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/Using_ManagingPasswordPolicies.html |
| **Recommended Action** | Update the password policy to require the use of lowercase letters |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for IAM. </br><img src="/resources/aws/iam/password-requires-lowercase/step2.png"/>
3. Scroll down the left navigation panel and choose "Account Settings". </br><img src="/resources/aws/iam/password-requires-lowercase/step3.png"/>
4. On the Account Settings page, click on the "Change" under the "Password Policy".</br> <img src="/resources/aws/iam/password-requires-lowercase/step4a.png"/>
5. Under the "Password Policy" configuration panel scroll down and check the "Require at least one lowercase letter". If the checkbox is not selected than the password policy does not requires at least one lowercase letter.</br><img src="/resources/aws/iam/password-requires-lowercase/step4.png"/>
6. Repeat steps number 3 and 4 to ensures password policy requires at least one lowercase letter.</br>
7. Click on the checkbox next to "Require at least one lowercase letter" so "Password Policy" requires at least one lowercase letter to make the password more strong and secure. </br> <img src="/resources/aws/iam/password-requires-lowercase/step6.png"/>
8. Click on the "Save Changes" button to make the necessary changes.</br><img src="/resources/aws/iam/password-requires-lowercase/step7a.png"/>
