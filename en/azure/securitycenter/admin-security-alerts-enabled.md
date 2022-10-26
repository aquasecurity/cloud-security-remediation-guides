[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Security Center / Admin Security Alerts Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Admin Security Alerts Enabled |
| **Cloud** | AZURE |
| **Category** | Security Center |
| **Description** | Ensures that security alerts are configured to be sent to admins |
| **More Info** | Enabling security alerts to be sent to admins ensures that detected vulnerabilities and security issues are sent to the subscription admins for quick remediation. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-provide-security-contact-details |
| **Recommended Action** | Ensure that security alerts are configured to be sent to subscription owners. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Microsoft Defender for Cloud". </br> <img src="/resources/azure/securitycenter/admin-security-alerts-enabled/step2.png"/>
3. On the "Microsoft Defender for Cloud" page scroll down the left navigation panel and choose "Environment Settings".</br> <img src="/resources/azure/securitycenter/admin-security-alerts-enabled/step3.png"/>
4. On the "Environment Settings" page, select the "Subscription" by clicking on the "Name".</br> <img src="/resources/azure/securitycenter/admin-security-alerts-enabled/step4.png"/>
5. Under the "Settings | Defender plans " page, click on the "Email Notifications"</br> <img src="/resources/azure/securitycenter/admin-security-alerts-enabled/step5.png"/>
6. On the "Settings | Email notifications" page under "Email recipients" if the "Additional email addresses (separated by commas)" is empty and only "owner" is selected in "All users with the following roles" then the security alerts are not configured to be sent to admins.</br> <img src="/resources/azure/securitycenter/admin-security-alerts-enabled/step6.png"/>
7. Under "Email recipients", click the dropdown for "All users with the following roles" and check mark "AccountAdmin and Service"Admin" along with owner and enter one or more than one "Email addressess" separated by "comma in section "Additional email addresses (separated by commas)".</br> <img src="/resources/azure/securitycenter/admin-security-alerts-enabled/step7.png"/>
8. Under "Notification types" select "High" from the dropdown next to "Notify about alerts with the following severity (or higher). Click on the "Save" button to make the changes.</br> <img src="/resources/azure/securitycenter/admin-security-alerts-enabled/step8.png"/>
9. Repeat step number 3 - 8 to ensure that security alerts are configured to be sent to subscription owners.</br>
