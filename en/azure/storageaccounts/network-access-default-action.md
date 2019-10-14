[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Network Access Default Action

## Quick Info

| | |
|-|-|
| **Plugin Title** | Network Access Default Action |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures that Storage Account access is restricted to trusted networks |
| **More Info** | Storage Accounts should be configured to accept traffic only from trusted networks. By default, all networks are selected but can be changed when creating a new storage account or in the firewall settings. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/common/storage-network-security |
| **Recommended Action** | Configure the firewall of each Storage Account to allow access only from known virtual networks. |

## Detailed Remediation Steps

