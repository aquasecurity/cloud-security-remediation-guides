[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Security Center / Security Contact Additional Email

## Quick Info

| | |
|-|-|
| **Plugin Title** | Security Contact Additional Email |
| **Cloud** | AZURE |
| **Category** | Security Center |
| **Description** | Ensure Additional email addresses is Configured with a Security Contact Email |
| **More Info** | Microsoft Defender for Cloud emails the Subscription Owner to notify them about security alerts. Adding your Security Contact\'s email address to the Additional email addresses field ensures that your organization\'s Security Team is included in these alerts. This ensures that the proper people are aware of any potential compromise in order to mitigate the risk in a timely fashion. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/defender-for-cloud/configure-email-notifications |
| **Recommended Action** | Modify security contact information and add additional email |

## Detailed Remediation Steps

1. Login to the Microsoft Azure Management Console.
2. In the search bar at the top search for defender for cloud and click on "Microsoft Defender for Cloud".<br/> <img src="/resources/azure/securitycenter/security-contact-additional-email/step2.png"/>
3. On the defender for cloud page, choose on the "Envoirnment Settings" from the left navigation panel.<br/> <img src="/resources/azure/securitycenter/security-contact-additional-email/step3.png"/>
4. On envoirnment settings page select the appropriate Management Group, Subscription, or Workspace.<br/> <img src="/resources/azure/securitycenter/security-contact-additional-email/step4.png"/>
5. On Settings page choose "Email Notification" from the left navigation panel.<br/> <img src="/resources/azure/securitycenter/security-contact-additional-email/step5.png"/>
6. Enter a valid security contact email address (or multiple addresses separated by commas) in the 'Additional email addresses' field and Click Save<br/> <img src="/resources/azure/securitycenter/security-contact-additional-email/step6.png"/>



