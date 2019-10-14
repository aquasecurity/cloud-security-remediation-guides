[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Object Store / Object Store Policy Protection

## Quick Info

| | |
|-|-|
| **Plugin Title** | Object Store Policy Protection |
| **Cloud** | ORACLE |
| **Category** | Object Store |
| **Description** | Ensure Policy statements have deletion protection for Object Store Services unless it is an administrator group. |
| **More Info** | Adding deletion protection to Oracle Object Store policies mitigates unintended deletion of Object Store Services by unauthorized users or groups. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Security/Reference/dbaas_security.htm |
| **Recommended Action** | When writing policies, avoid blanket statements, and add a where statement with the line request.permission != {OBJECT_DELETE, BUCKET_DELETE} . |

## Detailed Remediation Steps

