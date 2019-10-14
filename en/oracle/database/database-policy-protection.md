[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Database / Database Policy Protection

## Quick Info

| | |
|-|-|
| **Plugin Title** | Database Policy Protection |
| **Cloud** | ORACLE |
| **Category** | Database |
| **Description** | Ensure Policy statements have deletion protection for Database Systems, Databases, and Database Homes unless it is an administrator group. |
| **More Info** | Adding deletion protection to Oracle Database policies mitigates unintended deletion of Database Services by unauthorized users or groups. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Security/Reference/dbaas_security.htm |
| **Recommended Action** | When writing policies, avoid blanket statements, and add a where statement with the line request.permission != {DB_SYSTEM_DELETE, DATABASE_DELETE, DB_HOME_DELETE} . |

## Detailed Remediation Steps

