[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Trusted MS Access Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Trusted MS Access Enabled |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures that Trusted Microsoft Services Access is enabled on Storage Accounts |
| **More Info** | Enabling firewall rules on Storage Accounts blocks all access by default. To ensure that Microsoft and Azure services that connect to the Storage Account still retain access, trusted Microsoft services should be allowed to access the storage account. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/common/storage-network-security |
| **Recommended Action** | For each Storage Account, configure an exception for trusted Microsoft services. |

## Detailed Remediation Steps

