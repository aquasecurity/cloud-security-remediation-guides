[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / File Storage / File Storage Policy Protection

## Quick Info

| | |
|-|-|
| **Plugin Title** | File Storage Policy Protection |
| **Cloud** | ORACLE |
| **Category** | File Storage |
| **Description** | Ensures policy statements have deletion protection for file storage services unless it is an administrator group. |
| **More Info** | Adding deletion protection to Oracle file storage policies mitigates unintended deletion of file storage services by unauthorized users or groups. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Security/Reference/filestorage_security.htm |
| **Recommended Action** | When writing policies, avoid blanket statements, and add a where statement with the line request.permission != {FILE_SYSTEM_DELETE, MOUNT_TARGET_DELETE, EXPORT_SET_DELETE} . |

## Detailed Remediation Steps

