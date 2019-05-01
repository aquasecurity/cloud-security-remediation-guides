[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Queue Service / Queue Service All Access ACL

## Quick Info

| | |
|-|-|
| **Plugin Title** | Queue Service All Access ACL |
| **Cloud** | AZURE |
| **Category** | Queue Service |
| **Description** | Ensures Queues do not allow full write, delete, or read ACL permissions |
| **More Info** | Queues can be configured to allow to read, write or delete objects. This option should not be configured unless there is a strong business requirement. |
| **AZURE Link** | httphttps://docs.microsoft.com/en-us/azure/storage/queues/storage-quickstart-queues-portal |
| **Recommended Action** | Disable global read/write/detele policies on all Queues and ensure the ACL is configured with least privileges. |

## Detailed Remediation Steps

