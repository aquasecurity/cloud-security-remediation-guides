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

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Storage account. </br> <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step3.png"/>
4. Scroll down the selected "Storage account" navigation panel and in "Settings" click on the "Encryption" option.</br> <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step4.png"/>
5. On the "Encryption" tab click on the "Use your own key" option. Choose "Select from Key Vault" option and if there is no active key then encryption is not configured in "Storage accounts." </br>  <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Storage accounts" in the Azure account. </br>
7. Navigate to the "Storage accounts", select the "Storage account" and click on the "Name", select the "Encryption" under "Settings."</br> <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step7.png"/>
8. Click on the "Use your own key" option and choose the "Select from Key Vault" option. Click on the "Select" option under "Key vault."</br> <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step8.png"/>
9. On the "Key vault" tab select the exisiting "Key vault" or click on the "Create a new vault" option and provide the "Name" and other details and click on the "Create" button at the bottom of the page. </br> <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step9.png"/>
10. Click on the "Select" option under the "Encryption key" to select the existing key in the vault or create a new key. </br> <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step10.png"/>
11. Provide a "Name" to the new key, select the "Activation date" option and choose the date as per the requirement and click on the "Create" button at the bottom. </br> <img src="/resources/azure/storageaccounts/storage-accounts-encryption/step11.png"/>
12. Repeat steps number 7 - 11 to ensures encryption is properly configured in "Storage accounts" to protect data-at-rest and meet compliance requirements.</br>
