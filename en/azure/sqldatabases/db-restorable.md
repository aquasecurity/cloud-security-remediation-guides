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

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for SQL databases. </br> <img src="/resources/azure/sqldatabases/db-restorable/step2.png"/>
3. On the "SQL database" page, select the SQL database that needs to be examine.</br> <img src="/resources/azure/sqldatabases/db-restorable/step3.png"/>
4. On the selected "SQL database" page, scroll down the left navigation panel and select "Overview" option.</br> <img src="/resources/azure/sqldatabases/db-restorable/step4.png"/>
5. On the "Overview" page, click on the "Restore" option at the top.</br> <img src="/resources/azure/sqldatabases/db-restorable/step5.png"/>
6. On the "Restore" page, scroll down and check the "Earliest restore point" under the "Point-in-time" and if it's showing "No restore point available" then the selected "SQL database" cannot be restored to a recent point.</br> <img src="/resources/azure/sqldatabases/db-restorable/step6.png"/>
7. Repeat steps number 2 - 6 to verify other "SQL databases" in the account.</br>
8. Navigate to "SQL databases", on the "SQL database" page select the "SQL database", scroll down the left navigation panel and choose "Overview." </br> <img src="/resources/azure/sqldatabases/db-restorable/step8.png"/>
9. Click on the "Restore" option at the top. </br> <img src="/resources/azure/sqldatabases/db-restorable/step9.png"/>
10. On the "Restore" page, select the "Source", "Restore Point" and "Pricing tier" as per the requirements and click on "OK" button at the bottom.</br> <img src="/resources/azure/sqldatabases/db-restorable/step10.png"/>
11. Repeat steps number 8 - 10 to ensure that each SQL database has automated backups configured with a sufficient retention period and that the last known backup operation completes successfully.</br>
