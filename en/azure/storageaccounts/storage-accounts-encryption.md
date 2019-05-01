[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Storage Accounts Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | Storage Accounts Encryption |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures encryption is properly configured in storage accounts to protect data-at-rest and meet compliance requirements. |
| **More Info** | Storage accounts can be configured to encrypt data-at-rest, by default Azure will create a set of keys to encrypt your storage account, but the recommended approach is to create your own keys using Azure Key Vault. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/common/storage-service-encryption-customer-managed-keys |
| **Recommended Action** | Go to your Storage Account, select Encryption, and check the box to use your own key, then select Key Vault, create a new vault if needed; then select Encryption key and create a new key if needed, at a minimum, set an activation date for your key to help with your key rotation policy, click Save when done. |

## Detailed Remediation Steps

