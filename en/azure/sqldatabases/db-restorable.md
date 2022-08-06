[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Databases / DB Restorable

## Quick Info

| | |
|-|-|
| **Plugin Title** | DB Restorable |
| **Cloud** | AZURE |
| **Category** | SQL Databases |
| **Description** | Ensures SQL Database instances can be restored to a recent point |
| **More Info** | Automated backups of SQL databases with recent restore points help ensure that database recovery operations can occur without significant data loss. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/sql-database/sql-database-recovery-using-backups |
| **Recommended Action** | Ensure that each SQL database has automated backups configured with a sufficient retention period and that the last known backup operation completes successfully. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "SQL databases". </br> <img src="/resources/azure/sqldatabases/db-restorable/step2.png"/>
3. On the "SQL database" page, select the SQL database that needs to be examined and click on its name to reach its configuration page.</br> <img src="/resources/azure/sqldatabases/db-restorable/step3.png"/>
4. On the selected "SQL database" page, scroll down the left navigation panel and select "Overview" and click on "Restore" button at the top.</br> <img src="/resources/azure/sqldatabases/db-restorable/step4.png"/>
5. On the "Create SQL Database - Restore database" page, select the desired configuration and click "Review + Create" at the bottom.</br> <img src="/resources/azure/sqldatabases/db-restorable/step4.png"/>
6. On the "Review + Create" page, click on the "Create" button.</br> <img src="/resources/azure/sqldatabases/db-restorable/step6.png"/>
7. On the restored database, verify that all data matches with the current database.
8. Repeat steps number 4 - 7 to ensure that each SQL database has automated backups configured with a sufficient retention period and that the last known backup operation completes successfully.</br>
