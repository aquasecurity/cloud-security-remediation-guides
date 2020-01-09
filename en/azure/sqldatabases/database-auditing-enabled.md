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

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for SQL databases. </br> <img src="/resources/azure/sqldatabases/database-auditing-enabled/step2.png"/>
3. On the "SQL database" page, select the SQL database that needs to be examine.</br><img src="/resources/azure/sqldatabases/database-auditing-enabled/step3.png"/>
4. On the selected "SQL database" page, scroll down the left navigation panel and select "Auditing" under the "Security."</br> <img src="/resources/azure/sqldatabases/database-auditing-enabled/step4.png"/>
5. On the "Auditing configuration page", verify the "Auditing" staus. If it's set to "OFF" then "SQL database Auditing" is not enabled for the selected "SQL database." </br> <img src="/resources/azure/sqldatabases/database-auditing-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "SQL databases" in the account.</br>
7. Navigate to "SQL databases", on the "SQL database" page select the "SQL database", scroll down the left navigation panel and choose "Auditing" under the "Security."</br> <img src="/resources/azure/sqldatabases/database-auditing-enabled/step7.png"/>
8. On the "Auditing configuration page", click on the "ON" option next to "Auditing" and select the "Audit log destination" from the "Storage /Log Analytics/ Event Hub" as per the availability.</br>  <img src="/resources/azure/sqldatabases/database-auditing-enabled/step8.png"/>
9. Click on the "Save" button at the top to make the changes.</br>  <img src="/resources/azure/sqldatabases/database-auditing-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to ensure that auditing is enabled for each SQL database.</br>
