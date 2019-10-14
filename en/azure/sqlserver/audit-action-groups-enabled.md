[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Server / Audit Action Groups Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Audit Action Groups Enabled |
| **Cloud** | AZURE |
| **Category** | SQL Server |
| **Description** | Ensures that SQL Server Audit Action and Groups is configured properly |
| **More Info** | SQL Server Audit Action and Groups should be configured to at least include SUCCESSFUL_DATABASE_AUTHENTICATION_GROUP, FAILED_DATABASE_AUTHENTICATION_GROUP and BATCH_COMPLETED_GROUP. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/sql-database/sql-database-auditing |
| **Recommended Action** | If SQL Server Audit Action and Groups is not configured properly when enabling Auditing, these settings must be configured in Powershell. |

## Detailed Remediation Steps

