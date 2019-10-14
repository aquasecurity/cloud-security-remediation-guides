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

