[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Defender / Security Contacts Enabled

## Quick Info

| | |
|-|----------------------------------------------------------------------------------------------------------------------------------------------|
| **Plugin Title** | Security Contacts Enabled |
| **Cloud** | AZURE |
| **Category** | Defender |
| **Description** | Ensures that defender contact phone number and email address are set |
| **More Info** | Setting defender contacts ensures that any defender incidents detected by Azure are sent to a defender team equipped to handle the incident. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/defender-for-cloud/configure-email-notifications |
| **Recommended Action** | Ensure that email notifications are configured for the subscription from the Microsoft Defender for Cloud. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Microsoft Defender for Cloud". </br> <img src="/resources/azure/defender/security-contacts-enabled/step2.png"/>
3. On the "Microsoft Defender for Cloud" page, scroll down the left navigation panel and choose "Environment Settings". </br> <img src="/resources/azure/defender/security-contacts-enabled/step3.png"/>
4. On the "Environment Settings" page, select the "Subscription" by clicking on the "Name". </br> <img src="/resources/azure/defender/security-contacts-enabled/step4.png"/>
5. Under the "Settings | Defender plans " page, click on the "Email Notifications". </br> <img src="/resources/azure/defender/security-contacts-enabled/step5.png"/>
6. On the "Settings | Email notifications" page under "Email recipients" if the "Additional email addresses (separated by commas)" is empty and only "owner" is selected in "All users with the following roles" then the defender alerts are not configured to be sent to the admins. </br> <img src="/resources/azure/defender/security-contacts-enabled/step6.png"/>
7. Under "Email recipients", click the dropdown for "All users with the following roles" and check mark "AccountAdmin and "ServiceAdmin" along with owner and enter one or more than one "Email addresses" separated by "comma in section "Additional email addresses (separated by commas)". </br> <img src="/resources/azure/defender/security-contacts-enabled/step7.png"/>
8. Under "Notification types" select "High" from the dropdown next to "Notify about alerts with the following severity (or higher). Click on the "Save" button to make the changes. </br> <img src="/resources/azure/defender/security-contacts-enabled/step8.png"/>
9. Repeat step number 3 - 8 to ensure to ensure that email notifications are configured to be sent. </br>