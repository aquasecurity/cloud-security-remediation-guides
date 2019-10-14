[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Compute / Instance Policy Protection

## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance Policy Protection |
| **Cloud** | ORACLE |
| **Category** | Compute |
| **Description** | Ensure Policy statements have deletion protection for Compute Instances unless it is an administrator group. |
| **More Info** | Adding deletion protection to Oracle Compute Instance policies mitigates unintended deletion of instances by unauthorized users or groups. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Security/Reference/iam_security.htm |
| **Recommended Action** | When writing policies, avoid blanket statements, and add a where statement with the line request.permission != INSTANCE_DELETE. |

## Detailed Remediation Steps

