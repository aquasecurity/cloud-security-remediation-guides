[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Blob Service Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | Blob Service Encryption |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures encryption is properly configured for Blob Services |
| **More Info** | Blob Services can be configured to encrypt data-at-rest. By default Azure will create a set of keys to encrypt Blob Services, but the recommended approach is to create your own keys using Azure Key Vault. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/common/storage-service-encryption |
| **Recommended Action** | Ensure that Blob Service is configured to use a customer-provided key vault key. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Storage accounts."</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step2.png"/>
3. On the "Storage account" page, select the account by clicking on its "Name".</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step3.png"/>
4. On the configuration page scroll down the left navigation panel and select "Containers" under "Data Storage." </br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step4.png"/>
5. Select the "Container" on the "Containers" page.</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step5.png"/>
6. Scroll down the "Storage account" navigation panel and select "Encryption" under "Security + networking."</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step6.png"/>
7. On the "Encryption page" scroll down and check the "Encryption type". If "Microsoft-managed keys" is selected, then "BYOK encryption" is not configured in the Blob Service Encryption.</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step7.png"/>
8. To enable "BYOK encryption" select "Encryption type" as "Customer-managed keys". In the "Encryption key" select option "Select from key vault". </br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step8.png"/>
9. In the "Key Vault and key" click on the blue hughlighted text "Select a key vault and key". </br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step9.png"/>
10. On the "Select a key" page, select "Key store type" as "Key vault". In the "Key vault" and "key" options select the key vault and key from the dropdown or you can create your own key vault and key. Click "Select" button at the end to save the selected options.</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step10.png"/>
11. Click on the "Save" button at the end to make the changes.</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step11.png"/>
12. Repeat steps number 3 - 11 to ensure the Storage Account used by Blog Services is configured with a BYOK key.</br>
