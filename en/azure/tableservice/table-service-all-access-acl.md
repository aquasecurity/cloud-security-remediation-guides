[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Table Service / Table Service All Access ACL

## Quick Info

| | |
|-|-|
| **Plugin Title** | Table Service All Access ACL |
| **Cloud** | AZURE |
| **Category** | Table Service |
| **Description** | Ensures tables do not allow full write, delete, or read ACL permissions |
| **More Info** | Table Service tables can be configured to allow to read, write or delete on objects. This option should not be configured unless there is a strong business requirement. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/tables/table-storage-quickstart-portal |
| **Recommended Action** | Disable global read, write, and delete policies on all tables and ensure the ACL is configured with least privileges. |

## Detailed Remediation Steps

