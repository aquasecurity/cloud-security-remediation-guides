[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / File Service Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | File Service Encryption |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures data encryption is enabled for File Services |
| **More Info** | File Service encryption protects your data at rest. Azure Storage encrypts your data and automatically decrypts it for you as you access it. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/common/storage-service-encryption |
| **Recommended Action** | Ensure that data encryption is enabled for each File Service. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Storage accounts".</br> <img src="/resources/azure/storageaccounts/file-service-encryption/step2.png"/>
3. On the "Storage account" page, scroll down the left navigation panel and choose "File shares" under "Data Storage". </br> <img src="/resources/azure/storageaccounts/file-service-encryption/step3.png"/>
4. Select the "File share" on the "File sharing" page and check the storage account name at the top. File shares are a part of the Storage container. So to ensure encryption is properly configured for File Shares we have to check the encryption of the corresponding container </br> <img src="/resources/azure/storageaccounts/file-service-encryption/step4.png"/>
5. Navigate to "Storage account", select the corresponding "Storage account", scroll down the left navigation panel and choose "Encryption" under "Security + networking".</br> <img src="/resources/azure/storageaccounts/file-service-encryption/step5.png"/>
6. On the "Encryption page" scroll down and check the "Encryption type". If "Microsoft-managed keys" is selected, then "BYOK encryption" is not configured in the File Service Encryption.</br> <img src="/resources/azure/storageaccounts/file-service-encryption/step6.png"/>
7. To enable "BYOK encryption" select "Encryption type" as "Customer-managed keys". In the "Encryption key" select option "Select from key vault". <img src="/resources/azure/storageaccounts/file-service-encryption/step7.png"/></br>
8. In the "Key Vault and key" click on the blue hughlighted text "Select a key vault and key".<img src="/resources/azure/storageaccounts/file-service-encryption/step8.png"/></br>
9. On the "Select a key" page, select "Key store type" as "Key vault". In the "Key vault" and "key" options, select the key vault and key from the dropdown or you can create your own key vault and key. Click "Select" button at the end to save the selected options.<img src="/resources/azure/storageaccounts/file-service-encryption/step9.png"/></br>
10. Click on the "Save" button at the end to make the changes.<img src="/resources/azure/storageaccounts/file-service-encryption/step10.png"/></br>
11. Repeat step number 3 - 10 to ensure that data encryption is enabled for each File Service.</br>
