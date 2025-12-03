[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Storage Account Infrastructure Encryption Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Storage Account Infrastructure Encryption Enabled |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensure that Azure Storage accounts have infrastructure encryption enabled. |
| **More Info** | Azure Storage automatically encrypts all data in a storage account at the service level using 256-bit AES encryption. But customers who require higher levels of assurance that their data is secure can also enable 256-bit AES encryption at the Azure Storage infrastructure level for double encryption. Double encryption of Azure Storage data protects against a scenario where one of the encryption algorithms or keys may be compromised. In this scenario, the additional layer of encryption continues to protect your data. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/storage/common/infrastructure-encryption-enable |
| **Recommended Action** | Delete storage account and create new storage account with infrastructure encryption enabled. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Storage accounts."</br> <img src="/resources/azure/storageaccounts/infrastructure-encryption-enabled/step2.png"/>
3. On Storage Accounts page Click on Create from navigation bar on top of the page.</br> <img src="/resources/azure/storageaccounts/infrastructure-encryption-enabled/step3.png"/>
4. Enter the required information and under the "Encryption" tab check the "Enable infrastructure encryption" box.</br> <img src="/resources/azure/storageaccounts/infrastructure-encryption-enabled/step4.png"/>
5. After Adding the all required information and completing all steps Click on review at the bottom of the page and then Click Create.</br> <img src="/resources/azure/storageaccounts/infrastructure-encryption-enabled/step5.png"/>
6. By following the above mentioned steps you will be able to create storage account with infrastructure encryption enabled.