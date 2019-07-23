[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Security Center / Monitor Disk Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | Monitor Disk Encryption |
| **Cloud** | AZURE |
| **Category** | Security Center |
| **Description** | Ensures Disk Encryption monitoring is enabled in Security Center. |
| **More Info** | When this setting is enabled, Security Center audits disk encryption in all virtual machines (Windows and Linux as well) to enhance data protection at rest. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-policy-definitions |
| **Recommended Action** | 1. Go to Azure Security Center 2. Click On the security policy to Open Policy Management Blade. 3. Click Subscription View 4. Click on Subscription Name to open Security Policy Blade for the Subscription. 5. Expand Compute And Apps 6. Ensure that Disk Encryption is not set to Disabled |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Security Center. </br> <img src="/resources/azure/securitycenter/monitor-disk-encryption/step2.png"/>
3. Scroll down the "Security Center" navigation panel and select the "Security policy" option under "POLICY & COMPLIANCE."</br> <img src="/resources/azure/securitycenter/monitor-disk-encryption/step3.png"/>
4. On the "Policy Management" page under "Name" column select the "Subscription Name" that needs to be verified.</br> <img src="/resources/azure/securitycenter/monitor-disk-encryption/step4.png"/>
5. On the "Security Policy" page scroll down the "Compute And Apps" section and check the "Disk encryption should be applied on virtual machines". If it's set to "Disabled" then "Disk Encryption monitoring" is not enabled on the selected "Subscription."</br> <img src="/resources/azure/securitycenter/monitor-disk-encryption/step5.png"/>
6. Repeat steps number 2 - 5 to check other "Subscriptions" under the "Security Center."</br>
7. Navigate to the "Security Center", select the "Security policy" and under "Policy Management" seelct the "Subscription" that needs to enable the "Disk Encryption monitoring."</br> <img src="/resources/azure/securitycenter/monitor-disk-encryption/step7.png"/>
8. Select the "Subscription" link under the "Security policy" at the top to get into the configuration settings. </br> <img src="/resources/azure/securitycenter/monitor-disk-encryption/step8.png"/>
9. Scroll down the page and under "Parameter" choose the "Disk encryption should be applied on virtual machines" and select the "AuditIfNotExists" option from the dropdown menu and click on the "Save" button at the bottom to make the necessary changes.</br> <img src="/resources/azure/securitycenter/monitor-disk-encryption/step9.png"/>
10. Repeat steps number 7 - 9 to ensures "Disk Encryption monitoring" is enabled in Security Center.</br>
