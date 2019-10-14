[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / File Service / File Service All Access ACL

## Quick Info

| | |
|-|-|
| **Plugin Title** | File Service All Access ACL |
| **Cloud** | AZURE |
| **Category** | File Service |
| **Description** | Ensures file shares do not allow full write, delete, or read ACL permissions |
| **More Info** | File shares can be configured to allow to read, write, or delete permissions from a share. This option should not be configured unless there is a strong business requirement. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/files/storage-how-to-create-file-share#create-a-file-share-through-the-azure-portal |
| **Recommended Action** | Disable global read, write, and delete policies on all file shares and ensure the share ACL is configured with least privileges. |

## Detailed Remediation Steps

