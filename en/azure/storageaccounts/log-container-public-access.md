[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Log Container Public Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Log Container Public Access |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensure that the Activity Log Container does not have public read access. |
| **More Info** | Enabling private access only on the Activity Log Storage Container ensures that log data is secured and only accessible from within, following security best practices. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/blobs/storage-manage-access-to-resources |
| **Recommended Action** | 1. Enter the activity log service. 2. Choose the export option. 3. Note the storage container in use. 4. Enter the storage account in use by navigating to the storage accounts service. 5. Select the Blob blade under Blob Service. 6. Select insights-operational-logs. 7. Click on Access Level and ensure that access is set to private. |

## Detailed Remediation Steps

