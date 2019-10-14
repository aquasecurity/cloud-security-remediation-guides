[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Log Storage Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | Log Storage Encryption |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures BYOK encryption is properly configured in the Activity Log Storage Account. |
| **More Info** | Storage accounts can be configured to encrypt data-at-rest, by default Azure will create a set of keys to encrypt your storage account, but the recommended approach is to create your own keys using Azure Key Vault. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/common/storage-service-encryption-customer-managed-keys |
| **Recommended Action** | 1. Enter the activity log service. 2. Choose the export option. 3. Note the storage container in use. 4. Enter the storage account in use by navigating to the storage accounts service. 5. Navigate to encryption and enable Use Your Own Key. |

## Detailed Remediation Steps

