[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Databases / Database Auditing Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Database Auditing Enabled |
| **Cloud** | AZURE |
| **Category** | SQL Databases |
| **Description** | Ensures that SQL Database Auditing is enabled |
| **More Info** | Enabling SQL Database Auditing ensures that all database activities are being logged properly, including potential malicious activity. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-enable-auditing-on-sql-databases |
| **Recommended Action** | Ensure that auditing is enabled for each SQL database. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "SQL databases". </br> <img src="/resources/azure/sqldatabases/database-auditing-enabled/step2.png"/>
3. On the "SQL database" page, select the SQL database that needs to be examined and click on its "Name" to reach its configuration page.</br><img src="/resources/azure/sqldatabases/database-auditing-enabled/step3.png"/>
4. On the selected "SQL database" page, scroll down the left navigation panel and select "Auditing" under "Security".</br> <img src="/resources/azure/sqldatabases/database-auditing-enabled/step4.png"/>
5. On the "Auditing configuration page", verify the "Enable Azure SQL Auditing" staus. If it's set to "OFF" then "SQL database Auditing" is not enabled for the selected "SQL database." </br> <img src="/resources/azure/sqldatabases/database-auditing-enabled/step5.png"/>
6. To enable Auditing for SQL database, on the "Auditing configuration page", turn the toggle status to "ON" and under "Audit log destination select from the "Storage /Log Analytics/ Event Hub" as per the availability.</br>  <img src="/resources/azure/sqldatabases/database-auditing-enabled/step6.png"/>
7. Click on the "Save" button at the top to make the necessary changes.</br>  <img src="/resources/azure/sqldatabases/database-auditing-enabled/step7.png"/>
8. Repeat steps number 3 - 7 to ensure that auditing is enabled for each SQL database.</br>
