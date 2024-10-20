[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Security Center / Security Contact Enabled for Subscription Owner

## Quick Info

| | |
|-|-|
| **Plugin Title** | Security Contact Enabled for Subscription Owner |
| **Cloud** | AZURE |
| **Category** | Security Center |
| **Description** | Ensure that security alert emails are enabled to subscription owners. |
| **More Info** | Enabling security alert emails to subscription owners ensures that they receive security alert emails from Microsoft. This ensures that they are aware of any potential security issues and can mitigate the risk in a timely fashion. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/defender-for-cloud/configure-email-notifications |
| **Recommended Action** | Modify security contact information and enable emails for subscription owners |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Microsoft Defender for Cloud". </br> <img src="/resources/azure/securitycenter/security-contact-role-set-owner/step2.png"/>
3. On the "Microsoft Defender for Cloud" page, scroll down the left navigation panel and choose "Environment Settings".</br> <img src="/resources/azure/securitycenter/security-contact-role-set-owner/step3.png"/>
4. On the "Environment Settings" page, select the "Subscription" by clicking on the "Name".</br> <img src="/resources/azure/securitycenter/security-contact-role-set-owner/step4.png"/>
5. Under the "Settings | Defender plans " page, click on the "Email Notifications"</br> <img src="/resources/azure/securitycenter/security-contact-role-set-owner/step5.png"/>
6. In the drop down of the 'All users with the following roles' field select 'Owner' and Click Save</br> <img src="/resources/azure/securitycenter/security-contact-role-set-owner/step6.png"/>