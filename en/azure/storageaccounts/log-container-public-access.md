[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Log Container Public Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Log Container Public Access |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures that the Activity Log Container does not have public read access |
| **More Info** | The container used to store Activity Log data should not be exposed publicly to avoid data exposure of sensitive activity logs. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/blobs/storage-manage-access-to-resources |
| **Recommended Action** | Ensure the access level for the storage account containing Activity Log data is set to private. |

## Detailed Remediation Steps

