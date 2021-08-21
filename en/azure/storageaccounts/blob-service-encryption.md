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
3. On the "Storage account" page, scroll down the left navigation panel and choose "Encryption" under the "Security + networking". </br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step3.png"/>
4. On the "Encryption page" scroll down and check whether Encryption type is set to "	Microsoft-managed keys" or "Customer-managed keys".</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step4.png"/>
5. Repeat steps number 2 - 4 to verify other "Blob Service Encryption" in the Azure account.</br>
6. Navigate to "Storage account", select the corresponding "Storage account", scroll down the left navigation panel and choose "Encryption."</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step6.png"/>
7. On the "Encyption page" select the "Customer-managed keys" and click on the "Select from Key Vault".</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step7.png"/>
8. On the "Key vault" option select the vault accordingly.</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step8.png"/>
9. On the "Encryption key" option select the key accordingly.</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step9.png"/>
10. Click on the "Save" option at the top to make the changes.</br> <img src="/resources/azure/storageaccounts/blob-service-encryption/step10.png"/>
11. Repeat steps number 8 - 10 to ensure the Storage Account used by Activity Logs is configured with a BYOK key.</br>
