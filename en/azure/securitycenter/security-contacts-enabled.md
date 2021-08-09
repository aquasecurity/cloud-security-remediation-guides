[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Security Center / Security Contacts Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Security Contacts Enabled |
| **Cloud** | AZURE |
| **Category** | Security Center |
| **Description** | Ensures that security contact phone number and email address are set |
| **More Info** | Setting security contacts ensures that any security incidents detected by Azure are sent to a security team equipped to handle the incident. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-provide-security-contact-details |
| **Recommended Action** | Ensure that email notifications are configured for the subscription from the Security Center. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Security Center. </br> <img src="/resources/azure/securitycenter/security-contacts-enabled/step2.png"/>
3. Scroll down the "Security Center" and select the "Security policy" option under "Management" in the left navigation panel.</br>
4. On the "Security Center - Pricing & settings" page, select the "Subscription" by clicking on the "Name."</br> <img src="/resources/azure/securitycenter/security-contacts-enabled/step4.png"/>
5. Under the "Settings - Pricing tier", click on the "Email Notifications" options on the left navigaton panel and if the "Email notification settings" are turned off along with "Phone number" then the "Security Contacts" are not enabled.</br> <img src="/resources/azure/securitycenter/security-contacts-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other Azure accounts for "Admin Security Alerts."</br>
7. Navigate to Security center, choose "Pricing and Settings", select the "Subscription" by clicking on the "Name" and click on the "Email Notifications" options.</br> <img src="/resources/azure/securitycenter/security-contacts-enabled/step7.png"/>
8. On the "Settings - Email notifications" page, enter the "Email address" and if there are more than 1 "Email address", then separate the email addresses by comma and select the Notification for alerts needed such as High severity.</br> <img src="/resources/azure/securitycenter/security-contacts-enabled/step8.png"/>
9. On the "Email notification settings" click on "ON" option next to "Send email notification for high severity alerts."Click on the Save button to make the changes.</br> <img src="/resources/azure/securitycenter/security-contacts-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to ensure that email notifications are configured for the subscription from the Security Center.</br>
