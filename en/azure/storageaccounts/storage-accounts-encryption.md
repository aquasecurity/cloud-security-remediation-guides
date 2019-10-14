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

