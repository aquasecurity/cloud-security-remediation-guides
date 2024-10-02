[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Defender / High Severity Alerts Enabled

## Quick Info

| |                                                                                                                                                             |
|-|-------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Plugin Title** | High Severity Alerts Enabled                                                                                                                                |
| **Cloud** | AZURE                                                                                                                                                       |
| **Category** | Defender                                                                                                                                                    |
| **Description** | Ensures that high severity alerts are enabled and properly configured.                                                                                                  |
| **More Info** | Enabling high severity alerts ensures that microsoft alerts for potential security issues are sent and allows for quick mitigation of the associated risks. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/defender-for-cloud/configure-email-notifications                                                     |
| **Recommended Action** | Enable email alert notification and configure its severity level.                                                                                              |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Microsoft Defender for Cloud". </br> <img src="/resources/azure/defender/high-severity-alerts-enabled/step2.png"/>
3. On the "Microsoft Defender for Cloud" page, scroll down the left navigation panel and choose "Environment Settings".</br> <img src="/resources/azure/defender/high-severity-alerts-enabled/step3.png"/>
4. On the "Environment Settings" page, select the "Subscription" by clicking on the "Name".</br> <img src="/resources/azure/defender/high-severity-alerts-enabled/step4.png"/>
5. Under the "Settings | Defender plans " page, click on the "Email Notifications. "</br> <img src="/resources/azure/defender/high-severity-alerts-enabled/step5.png"/>
6. On the "Settings | Email notifications" page under "Email recipients" if the "Additional email addresses (separated by commas)" is empty and only "owner" is selected in "All users with the following roles" then high severity alerts are not configured to be sent to the admins.</br> <img src="/resources/azure/defender/high-severity-alerts-enabled/step6.png"/>
7. Under "Email recipients", click the dropdown for "All users with the following roles" and check mark "AccountAdmin and "ServiceAdmin" along with owner and enter one or more than one "Email addresses" separated by "comma in section "Additional email addresses (separated by commas)".</br> <img src="/resources/azure/defender/high-severity-alerts-enabled/step7.png"/>
8. Under "Notification types" select "High" from the dropdown next to "Notify about alerts with the following severity (or higher). Click on the "Save" button to make the changes.</br> <img src="/resources/azure/defender/high-severity-alerts-enabled/step8.png"/>
9. Repeat step number 3 - 8 to ensure that high severity alerts are configured to be sent to subscription owners.</br>
