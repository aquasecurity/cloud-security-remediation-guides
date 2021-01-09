[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Object Store / Object Store Policy Protection

## Quick Info

| | |
|-|-|
| **Plugin Title** | Object Store Policy Protection |
| **Cloud** | ORACLE |
| **Category** | Object Store |
| **Description** | Ensure policy statements have deletion protection for object store services unless it is an administrator group. |
| **More Info** | Adding deletion protection to Oracle object store policies mitigates unintended deletion of object store services by unauthorized users or groups. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Object/Tasks/managingobjects.htm |
| **Recommended Action** | When writing policies, avoid blanket statements, and add a where statement with the line request.permission != {OBJECT_DELETE, BUCKET_DELETE} . |

## Detailed Remediation Steps

