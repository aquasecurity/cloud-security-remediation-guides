[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Databases / SQL DB Multiple AZ

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQL DB Multiple AZ |
| **Cloud** | AZURE |
| **Category** | SQL Databases |
| **Description** | Ensures that SQL Database instances are created to be cross-AZ for high availability |
| **More Info** | Creating SQL Database instances in a single availability zone creates a single point of failure for all systems relying on that database. All SQL Database instances should be created in multiple availability zones to ensure proper failover. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/sql-database/sql-database-high-availability#zone-redundant-configuration |
| **Recommended Action** | Ensure that each SQL Database is configured to be zone redundant. |

## Detailed Remediation Steps


