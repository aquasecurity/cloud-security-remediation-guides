[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Security Center / Monitor Blob Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | Monitor Blob Encryption |
| **Cloud** | AZURE |
| **Category** | Security Center |
| **Description** | Ensures that Blob Storage Encryption monitoring is enabled |
| **More Info** | When this setting is enabled, Security Center audits blob encryption in all storage accounts to enhance data at rest protection. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-policies |
| **Recommended Action** | Enable Adaptive Application Controls for Storage Accounts from the Azure Security Center by ensuring AuditIfNotExists setting is used for blob encryption. |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Security Center. </br> <img src="/resources/azure/securitycenter/monitor-blob-encryption/step2.png"/>
3. Scroll down the "Security Center" navigation panel and select the "Security policy" option under "POLICY & COMPLIANCE."</br> <img src="/resources/azure/securitycenter/monitor-blob-encryption/step3.png"/>
4. On the "Policy Management" page under "Name" column select the "Subscription Name" that needs to be verified.</br> <img src="/resources/azure/securitycenter/monitor-blob-encryption/step4.png"/>
5. On the "Security Policy" page scroll down the "Compute And Apps" section and check the "Adaptive Application Controls should be enabled on virtual machines". If it's set to "Disabled" then "Blob Storage Encryption monitoring" is not enabled on the selected "Subscription."</br> <img src="/resources/azure/securitycenter/monitor-blob-encryption/step5.png"/>
6. Repeat steps number 2 - 5 to check other "Subscriptions" under the "Security Center."</br>
7. Navigate to the "Security Center", select the "Security policy" and under "Policy Management" select the "Subscription" that needs to enable the "Adaptive Application Controls should be enabled on virtual machines."</br> <img src="/resources/azure/securitycenter/monitor-blob-encryption/step7.png"/>
8. Select the "Subscription" link under the "Security policy" at the top to get into the configuration settings. </br> <img src="/resources/azure/securitycenter/monitor-blob-encryption/step8.png"/>
9. Scroll down the page and under "Parameter" choose the "Adaptive Application Controls should be enabled on virtual machines" and select the "AuditIfNotExists" option from the dropdown menu and click on the "Save" button at the bottom to make the necessary changes.</br> <img src="/resources/azure/securitycenter/monitor-blob-encryption/step9.png"/>
10. Repeat steps number 7 - 9 to enable Adaptive Application Controls for Storage Accounts from the Azure Security Center by ensuring AuditIfNotExists setting is used for blob encryption.</br>
