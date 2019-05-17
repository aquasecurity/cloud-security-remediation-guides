[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Root MFA Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Root MFA Enabled |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures a multi-factor authentication device is enabled for the root account |
| **More Info** | The root account should have an MFA device setup to enable two-factor authentication. |
| **AWS Link** | http://docs.aws.amazon.com/general/latest/gr/managing-aws-access-keys.html |
| **Recommended Action** | Enable an MFA device for the root account and then use an IAM user for managing services |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Click on the AWS account name at the top on AWS management console and click on the "My Security Credentials" from the menu.</br><img src="/resources/aws/iam/root-mfa-enabled/step2.png"/>
3. On "Your Security Credentials" page scroll down and click on the "Multi-factor authentication (MFA)". Check the "Multi-factor authentication (MFA)" section for any active devices. If the  "Activate MFA" button is showing then a multi-factor authentication device is not enabled for the root account.</br><img src="/resources/aws/iam/root-mfa-enabled/step3.png"/>
4. Repeat steps number 2 and 3 to check another AWS account.</br>
5. On "Your Security Credentials" page scroll down and click on the "Multi-factor authentication (MFA)" and click on the "Activate MFA" button to enable a multi-factor authentication device.</br><img src="/resources/aws/iam/root-mfa-enabled/step5.png"/>
6. Click on the "Virtual MFA device" and click on "Continue". </br><img src="/resources/aws/iam/root-mfa-enabled/step6.png"/>
7. Now install the AWS MFA compatible application on mobile device or computer. Once the application is installed click on the "Show QR code" and scan the code with pre-installed application.</br><img src="/resources/aws/iam/root-mfa-enabled/step7.png"/>
8. Enter two consecutive MFA codes generated from application in "MFA code 1" and "MFA code 2" and click on the "Assign MFA" button.</br><img src="/resources/aws/iam/root-mfa-enabled/step8.png"/>
9. On successful setup will get the following message "You have successfully assigned virtual MFA". </br><img src="/resources/aws/iam/root-mfa-enabled/step9.png"/>
10. Now "Multi-factor authentication (MFA)" is enabled for the root account.</br>
