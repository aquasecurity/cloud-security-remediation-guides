[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Root Hardware MFA

## Quick Info

| | |
|-|-|
| **Plugin Title** | Root Hardware MFA |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures the root account is using a hardware MFA device |
| **More Info** | The root account should use a hardware MFA device for added security, rather than a virtual device which could be more easily compromised. |
| **AWS Link** | https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_mfa_enable_physical.html |
| **Recommended Action** | Enable a hardware MFA device for the root account and disable any virtual devices |

## Detailed Remediation Steps
1. Log in to the AWS Management Console using your root credentials.</br>
2. Click on the "Account name" option at the right corner of the management console and select Security Credentials from the dropdown menu.</br> <img src="/resources/aws/iam/root-hardware-mfa/step2.png"/>
3. On the "Security Credentials" page, click on the Multi-Factor Authentication (MFA).</br> <img src="/resources/aws/iam/root-hardware-mfa/step3.png"/>
4. On the MFA management panel, check for any enabled MFA device that has the attribute set "Hardware MFA". </br> <img src="/resources/aws/iam/root-hardware-mfa/step4.png"/>
5. Repeat steps number 2 - 4 to check other AWS root accounts.</br>
6. Click on the "Account name" option at the right corner of the management console and select Security Credentials from the dropdown menu.</br>
7. Click on the "Multi-Factor Authentication (MFA)" accordion tab to expand the MFA management panel.</br> <img src="/resources/aws/iam/root-hardware-mfa/step7.png"/>
8. Click on the "Activate MFA" button to initiate the MFA device setup process.</br> <img src="/resources/aws/iam/root-hardware-mfa/step8.png"/>
9. In the "Manage MFA device", select the "Other hardware MFA device" and click on the "Continue" button.</br> <img src="/resources/aws/iam/root-hardware-mfa/step9.png"/>
10. On the "Set up hardware MFA device", enter the "Serial number" and MFA Code 1 and MFA Code 2.</br> 
11. Click on the "Assign MFA" to complete the process.</br> 
12. Repeat steps number 6 - 11 to enable a hardware MFA device for the root account and disable any virtual devices.</br>



