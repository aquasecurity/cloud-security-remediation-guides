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

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Monitor". </br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step2.png"/>
3. On the left navigation panel, click on "Diagnostics Settigns" under "Settings".</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step3.png"/>
4. On the "Diagnostics settings" page, select the resource from the list with value "Enabled" in the "Diagnostic status" column by clicking on its name. </br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step4.png"/>
5. On the resource configuration page, copy the "Storage account" name for the "Activity Log".</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step5.png"/>
6. Now select the "Search resources, services, and docs" option at the top and search for "Storage accounts".</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step6.png"/>
7. Paste the "Storage account" name on the "Filter" option at the top, copied in Step 5 and select the corresponding "Storage account."</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step7.png"/>
8. Scroll down the "Storage account" navigation panel and select "Encryption" under "Security + networking."</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step8.png"/>
9. On the "Encryption page" scroll down and check the "Encryption type". If "Microsoft-managed keys" is selected, then "BYOK encryption" is not configured in the Activity log storage account.</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step9.png"/>
10. To enable "BYOK encryption" select "Encryption type" as "Customer-managed keys". In the "Encryption key" select option "Select from key vault". </br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step10.png"/>
11. In the "Key Vault and key" click on the blue hughlighted text "Select a key vault and key". </br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step11.png"/>
12. On the "Select a key" page, select "Key store type" as "Key vault". In the "Key vault" and "key" options select the key vault and key from the dropdown or you can create your own key vault and key. Click "Select" button at the end to save the selected options.</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step12.png"/>
13. Click on the "Save" button at the end to make the changes.</br> <img src="/resources/azure/storageaccounts/log-storage-encryption/step13.png"/>
14. Repeat steps number  4 - 13 to ensure the Storage Account used by Activity Logs is configured with a BYOK key for all resources with Diagnostic Status "Enabled".</br>
