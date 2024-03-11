[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Active Directory / Storage Accounts Minimum TLS Version

## Quick Info

| | |
|-|-|
| **Plugin Title** | Storage Accounts Minimum TLS Version |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures Microsoft Azure Storage Accounts are using the latest TLS version 1.2 to enforce stricter security measure. |
| **More Info** | Azure Storage accounts permit clients to send and receive data with the oldest version of TLS, TLS 1.0, and above. To enforce stricter security measures, you can configure your storage account to require that clients send and receive data with a newer version of TLS. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/common/transport-layer-security-configure-minimum-version |
| **Recommended Action** | Modify Storage Account configuration and set desired minimum TLS version |

## Detailed Remediation Steps

1. ASC Default policies should monitor for this by default. If no ASC Default policy found, this policy can be manually assigned and enabled. 
2. Log into the Microsoft Azure Management Console.
3. Select the "Search resources, services, and docs" option at the top and search for Storage Accounts.
4. Select the corresponding storage account by clicking on the "name" link.
5. Locate the Configuration option under Settings.
6. In the Minimum TLS Version section, select Version 1.2.
7. Save your changes. 
8. Repeat steps 4-7 for all other applicable Storage Accounts.
