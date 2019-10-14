[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Server / SQL Server Public Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQL Server Public Access |
| **Cloud** | AZURE |
| **Category** | SQL Server |
| **Description** | Ensures that SQL Servers do not allow public access |
| **More Info** | Unless there is a specific business requirement, SQL Server instances should not have a public endpoint and should only be accessed from within a VNET. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/sql-database/sql-database-security-overview/ |
| **Recommended Action** | Ensure that the firewall of each SQL Server is configured to prohibit traffic from the public 0.0.0.0 global IP address. |

## Detailed Remediation Steps

