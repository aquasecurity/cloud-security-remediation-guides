[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Defender / Security Contact Additional Email

## Quick Info

| |                                                                                                                                                                           |
|-|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Plugin Title** | Security Contact Additional Email                                                                                                                                               |
| **Cloud** | AZURE                                                                                                                                                                     |
| **Category** | Defender                                                                                                                                                                  |
| **Description** | Ensure Additional email addresses are configured with security contact email.                                                                                                            |
| **More Info** | 'Microsoft Defender for Cloud emails the Subscription Owner to notify them about security alerts. Adding your Security Contact's email address to the Additional email addresses field ensures that your organization's Security Team is included in these alerts. This ensures that the proper people are aware of any potential compromise in order to mitigate the risk in a timely fashion.                                            |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/defender-for-cloud/configure-email-notifications                                                                                 |
| **Recommended Action** | Modify security contact information and add additional emails. |

## Detailed Remediation Steps


1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Microsoft Defender for Cloud". </br> <img src="/resources/azure/defender/security-contacts-additional-email/step2.png"/>
3. On the "Microsoft Defender for Cloud" page, scroll down the left navigation panel and choose "Environment Settings".</br> <img src="/resources/azure/defender/security-contacts-additional-email/step3.png"/>
4. On the "Environment Settings" page, select the "Subscription" by clicking on the "Name".</br> <img src="/resources/azure/defender/security-contacts-additional-email/step4.png"/>
5. Under the "Settings | Defender plans " page, click on the "Email Notifications"</br> <img src="/resources/azure/defender/security-contacts-additional-email/step5.png"/>
6. On the "Settings | Email notifications" page under "Email recipients" if the "Additional email addresses (separated by commas)" is empty and only "owner" is selected in "All users with the following roles" then the defender alerts are not configured to be sent to the admins.</br> <img src="/resources/azure/defender/security-contacts-additional-email/step6.png"/>
7. Under "Email recipients", click the dropdown for "All users with the following roles" and check mark "AccountAdmin and "ServiceAdmin" along with owner and enter one or more than one "Email addresses" separated by "comma in section "Additional email addresses (separated by commas)".</br> <img src="/resources/azure/defender/security-contacts-additional-email/step7.png"/>
8. Under "Notification types" select "High" from the dropdown next to "Notify about alerts with the following severity (or higher). Click on the "Save" button to make the changes.</br> <img src="/resources/azure/defender/security-contacts-additional-email/step8.png"/>
9. Repeat step number 3 - 8 to ensure to ensure that email notifications are configured to be sent to subscription owners.</br>
