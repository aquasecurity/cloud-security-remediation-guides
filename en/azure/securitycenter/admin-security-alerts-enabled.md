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

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Security Center. </br> <img src="/resources/azure/securitycenter/admin-security-alerts-enabled/step2.png"/>
3. On the "Security Center" page scroll down the left navigation panel and choose "Pricing and Settings."</br> <img src="/resources/azure/securitycenter/admin-security-alerts-enabled/step3.png"/>
4. On the "Security Center - Pricing & settings" page, select the "Subscription" by clicking on the "Name."</br> <img src="/resources/azure/securitycenter/admin-security-alerts-enabled/step4.png"/>
5. Under the "Settings - Pricing tier", click on the "Email Notifications" options and if the "Email notification settings" are turned off then the security alerts are not configured to be sent to admins.</br> <img src="/resources/azure/securitycenter/admin-security-alerts-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other Azure accounts for "Admin Security Alerts."</br>
7. Navigate to Security center, choose "Pricing and Settings", select the "Subscription" by clicking on the "Name" and click on the "Email Notifications" options.</br> <img src="/resources/azure/securitycenter/admin-security-alerts-enabled/step7.png"/>
8. On the "Settings - Email notifications" page, enter the "Email address" and if there are more than 1 "Email address" then separate the email addresses by "comma."</br> <img src="/resources/azure/securitycenter/admin-security-alerts-enabled/step8.png"/>
9. On the "Email notification settings" click on "ON" option next to "Send email notification for high severity alerts."Click on the Save button to make the changes.</br> <img src="/resources/azure/securitycenter/admin-security-alerts-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to ensure that security alerts are configured to be sent to subscription owners.</br>
