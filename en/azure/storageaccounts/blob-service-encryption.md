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

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Storage account."</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step2.png"/>
3. On the "Storage account" page, scroll down the left navigation panel and choose "Containers" under the "Blob services." </br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step3.png"/>
4. Select the "Container" on the "Containers" page.</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step4.png"/>
5. Scroll down the "Storage account" navigation panel and choose "Encryption" option under the "Settings."</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step5.png"/>
6. On the "Encryption page" scroll down and check "Use your own key" setting configuration. If "Use your own key" setting checkbox is not checked, then "BYOK encryption" is not configured in the Blob Service Encryption.</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step6.png"/>
7. Repeat steps number 2 - 5 to verify other "Blob Service Encryption" in the Azure account.</br>
8. Navigate to "Storage account", select the corresponding "Storage account", scroll down the left navigation panel and choose "Encryption."</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step8.png"/>
9. On the "Encyption page" select the "Use your own key" and click on the "Select from Key Vault".</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step9.png"/>
10. On the "Key vault" option select the vault accordingly.</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step10.png"/>
11. On the "Encryption key" option select the key accordingly.</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step11.png"/>
12. Click on the "Save" option at the top to make the changes.</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step12.png"/>
13. Repeat steps number 8 - 12 to ensure the Storage Account used by Activity Logs is configured with a BYOK key.</br>
