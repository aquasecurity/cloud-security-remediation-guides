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
1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "SQL databases". </br> <img src="/resources/azure/sqldatabases/db-restorable/step2.png"/>
3. On the "SQL database" page, select the SQL database that needs to be examined and click on its name to reach its configuration page.</br> <img src="/resources/azure/sqldatabases/db-restorable/step3.png"/>
4. On the selected "SQL database" page, scroll down the left navigation panel and select "Overview" and click on "Restore" button at the top.</br> <img src="/resources/azure/sqldatabases/db-restorable/step4.png"/>
5. On the "Create SQL Database - Restore database" page, select the desired configuration and click "Review + Create" at the bottom.</br> <img src="/resources/azure/sqldatabases/db-restorable/step5.png"/>
6. On the "Review + Create" page, click on the "Create" button.</br> <img src="/resources/azure/sqldatabases/db-restorable/step6.png"/>
7. On the restored database, verify that all data matches with the current database.

