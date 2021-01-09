[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Block Storage / Block Storage Policy Protection

## Quick Info

| | |
|-|-|
| **Plugin Title** | Block Storage Policy Protection |
| **Cloud** | ORACLE |
| **Category** | Block Storage |
| **Description** | Ensure policy statements have deletion protection for block volumes unless it is an administrator group. |
| **More Info** | Adding deletion protection to Oracle block volume policies mitigates unintended deletion of block and boot volumes by unauthorized users or groups. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Security/Reference/iam_security.htm |
| **Recommended Action** | When writing policies, avoid blanket statements, and add a where statement with the line request.permission != {VOLUME_DELETE, VOLUME_BACKUP_DELETE, VOLUME_ATTACHMENT_DELETE}. |

## Detailed Remediation Steps

