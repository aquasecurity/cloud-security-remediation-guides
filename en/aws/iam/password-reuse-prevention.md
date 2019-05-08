[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Password Reuse Prevention

## Quick Info

| | |
|-|-|
| **Plugin Title** | Password Reuse Prevention |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures password policy prevents previous password reuse |
| **More Info** | A strong password policy enforces minimum length, expirations, reuse, and symbol usage |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/Using_ManagingPasswordPolicies.html |
| **Recommended Action** | Increase the minimum previous passwords that can be reused to 24. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for IAM. </br><img src="/resources/aws/iam/password-reuse-prevention/step2.png"/>
3. Scroll down the left navigation panel and choose "Account Settings". </br><img src="/resources/aws/iam/password-reuse-prevention/step3.png"/>
4. Under the "Password Policy" configuration panel scroll down and check the "Prevent password reuse ". If the checkbox is not selected than the password policy does not  prevents the reuse of password.</br><img src="/resources/aws/iam/password-reuse-prevention/step4.png"/>
5. Repeat steps number 3 and 4 to prevent reuse of password .</br>
6. Click on the checkbox next to "Prevent password reuse" so "Password Policy" prevents reuse of the older passwords. Enter the "Number of passwords to remember" to 24 . </br> <img src="/resources/aws/iam/password-reuse-prevention/step6.png"/>
7. Click on the "Apply Password Policy" button to make the necessary changes.</br><img src="/resources/aws/iam/password-reuse-prevention/step7.png"/>
