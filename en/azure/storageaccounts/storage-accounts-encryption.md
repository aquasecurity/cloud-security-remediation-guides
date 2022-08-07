[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Storage Accounts Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | Storage Accounts Encryption |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures encryption is enabled for Storage Accounts |
| **More Info** | Storage accounts can be configured to encrypt data-at-rest. By default Azure will create a set of keys to encrypt the storage account, but the recommended approach is to create your own keys using Azure Key Vault. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/common/storage-service-encryption-customer-managed-keys |
| **Recommended Action** | Ensure all Storage Accounts are configured with a BYOK key. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Storage account. </br> <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step3.png"/>
4. Scroll down the selected "Storage account" navigation panel and under "Settings" select "Encryption".</br> <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step4.png"/>
5. On the "Encryption" tab if "Microsoft-managed keys" is seleceted then encryption is not enabled for Storage Account.</br>  <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step5.png"/>
6. To ensure the selected storage Account is configured with a BYOK encryption select "Customer-managed keys". </br>  <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step6.png"/>
7. Under "Key Selection" select "Encryption key" as "Select from key vault". In the "Key vault and key" click on "Select a key vault and key".</br>  <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step7.png"/>
8. On the "Select a key" page, select "Key store type" as "Key vault" and select "Key vault" and "key" from the dropdown. Click "Select" at the bottom.</br>  <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step8.png"/>
9. Click "Save" button at the bottom.
10. Repeat steps 3 - 9 to ensure all Storage Accounts are configured with a BYOK key.
