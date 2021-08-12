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
3. Scroll down the "Security Center" and select the "Security policy" option under the "Management" on left navigation panel.</br> 
4. On the "Policy Management" page under "Name" column select the "Subscription Name" that needs to be verified.</br> <img src="/resources/azure/securitycenter/monitor-blob-encryption/step4.png"/>
5. In the "Security Policy" page scroll down and click on the "Azure Security Benchmark".</br> <img src="/resources/azure/securitycenter/monitor-blob-encryption/step5.png"/>
6. In the "Azure Security Benchmark" click on the Next button.</br> <img src="/resources/azure/securitycenter/monitor-blob-encryption/step6.png"/>
7. In the "Azure Security Benchmark", check for the "Adaptive Application Controls for defining safe applications should be enabled on your machines" Parameter and if it's set to "Disable" then the encryption is not enabled.</br> <img src="/resources/azure/securitycenter/monitor-blob-encryption/step7.png"/>
8. Repeat steps number 2 - 7 to check other "Subscriptions" under the "Security Center."</br>
9. Navigate to the "Security Center", select the "Security policy" and under "Policy Management" select the "Subscription" that needs to enable the "Adaptive Application  Controls for defining safe applications should be enabled on your machines."</br> <img src="/resources/azure/securitycenter/monitor-blob-encryption/step9.png"/>
10. In the "Security Policy" page scroll down and click on the "Azure Security Benchmark" and click on the "Next" button. </br> <img src="/resources/azure/securitycenter/monitor-blob-encryption/step10.png"/>
11. Scroll down the page and under "Parameter" choose the "Adaptive Application for defining safe applications should be enabled on your machines" and select the "AuditIfNotExists" option from the dropdown menu and click on the "Save" button at the bottom to make the necessary changes.</br> <img src="/resources/azure/securitycenter/monitor-blob-encryption/step11.png"/>
12. Repeat steps number 7 - 11 to enable Adaptive Application Controls for Storage Accounts from the Azure Security Center by ensuring AuditIfNotExists setting is used for blob encryption.</br>
