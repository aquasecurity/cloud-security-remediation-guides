[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Log Storage Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | Log Storage Encryption |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures BYOK encryption is properly configured in the Activity Log Storage Account |
| **More Info** | Storage accounts can be configured to encrypt data-at-rest. By default Azure will create a set of keys to encrypt the storage account, but the recommended approach is to create your own keys using Azure Key Vault. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/common/storage-service-encryption-customer-managed-keys |
| **Recommended Action** | Ensure the Storage Account used by Activity Logs is configured with a BYOK key. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Monitor. </br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step2.png"/>
3. Select the "Log Activity" on the "Monitor-Overview" page. </br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step3.png"/>
4. On the "Activity Log" page, click on the "Diagnostics Settigns" at the top.</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step4.png"/>
5. On the "Diagnostics settings" page, copy the "Storage account" name for the "Activity Log".</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step5.png"/>
6. Select the "Search resources, services, and docs" option at the top and search for "Storage account."</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step6.png"/>
7. Paste the "Storage account" name on the "Filter" option at the top, copied in Step 5 and select the corresponding "Storage account."</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step7.png"/>
8. Scroll down the "Storage account" navigation panel and choose "Encryption" option under the "Settings."</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step8.png"/>
9. On the "Encryption page" scroll down and check "Use your own key" setting configuration. If "Use your own key" setting checkbox is not checked, then "BYOK encryption" is not configured in the Activity Log Storage Account.</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step9.png"/>
10. Repeat steps number 2 - 9 to verify other "Log Storage Encryptions" in the Azure account.</br>
11. Navigate to "Storage account", select the corresponding "Storage account", scroll down the left navigation panel and choose "Encryption."</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step11.png"/>
12. On the "Encyption page" select the "Use your own key" and click on the "Select from Key Vault".</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step12.png"/>
13. On the "Key vault" option select the vault accordingly.</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step13.png"/>
14. On the "Encryption key" option select the key accordingly.</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step14.png"/>
15. Click on the "Save" option at the top to make the changes.</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step15.png"/>
16. Repeat steps number 11 - 15 to ensure the Storage Account used by Activity Logs is configured with a BYOK key.</br>
