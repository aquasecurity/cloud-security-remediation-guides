[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Active Directory / Blobs Soft Deletion Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Blobs Soft Deletion Enabled |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensure that soft delete feature is enabled for all Microsoft Storage Account blobs. |
| **More Info** | When soft delete for blobs is enabled for a storage account, blobs, blob versions, and snapshots in that storage account may be recovered after they are deleted, within a retention period that you specify. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/blobs/soft-delete-blob-overview |
| **Recommended Action** | Enable soft delete for blobs and set deletion retention policy to keep blobs for more than desired number of days. |

## Detailed Remediation Steps

1. ASC Default policies should monitor for this by default. If no ASC Default policy found, this policy can be manually assigned and enabled. 
2. Log into the Microsoft Azure Management Console.
3. Select the "Search resources, services, and docs" option at the top and search for Storage Accounts.
4. Select the corresponding storage account by clicking on the "name" link.
5. Locate the Data Protection option under Data management.
6. In the Recovery section, select Turn on soft delete for blobs.
7. Specify a retention period between 30 and 365 days.
8. Save your changes. 
9. Repeat steps 4-8 for all other applicable Storage Accounts.
