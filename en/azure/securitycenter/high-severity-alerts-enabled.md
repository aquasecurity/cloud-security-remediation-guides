[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Security Center / High Severity Alerts Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | High Severity Alerts Enabled |
| **Cloud** | AZURE |
| **Category** | Security Center |
| **Description** | Ensures that high severity alerts are enabled and properly configured. |
| **More Info** | Enabling high severity alerts ensures that microsoft alerts for potential security issues are sent and allows for quick mitigation of the associated risks. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/defender-for-cloud/configure-email-notifications |
| **Recommended Action** | Enable email alert notification and configure its severity level. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Microsoft Defender for Cloud". </br> <img src="/resources/azure/securitycenter/high-severity-alerts-enabled/step2.png"/>
3. On the "Microsoft Defender for Cloud" page, scroll down the left navigation panel and choose "Environment Settings".</br> <img src="/resources/azure/securitycenter/high-severity-alerts-enabled/step3.png"/>
4. On the "Environment Settings" page, select the "Subscription" by clicking on the "Name".</br> <img src="/resources/azure/securitycenter/high-severity-alerts-enabled/step4.png"/>
5. Under the "Settings | Defender plans " page, click on the "Email Notifications. "</br> <img src="/resources/azure/securitycenter/high-severity-alerts-enabled/step5.png"/>
6. Under "Notification types" select the check box next to "Notify about alerts with the following severity (or higher)" then select desired severity level from dropdown and Click save at top of the page..</br> <img src="/resources/azure/securitycenter/high-severity-alerts-enabled/step6.png"/>
