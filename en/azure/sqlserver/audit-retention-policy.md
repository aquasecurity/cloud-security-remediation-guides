[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Server / Audit Retention Policy

## Quick Info

| | |
|-|-|
| **Plugin Title** | Audit Retention Policy |
| **Cloud** | AZURE |
| **Category** | SQL Server |
| **Description** | Ensures that SQL Server Auditing retention policy is set to greater than 90 days |
| **More Info** | Enabling SQL Server Auditing ensures that all activities are being logged properly, including potentially-malicious activity. Having a long retention policy ensures that all logs are kept for auditing and legal purposes. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/sql-database/sql-database-auditing |
| **Recommended Action** | Ensure that the storage account retention policy for each SQL server is set to greater than 90 days. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "SQL Server".</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step2.png"/>
3. On the "SQL server" page, select the SQL server by clicking on the "Name" as a link.</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step3.png"/>
4. On the "SQL server" Overview page, scroll down and select the "Auditing" under the Security.</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step4.png"/>
5. On the "SQL server" Auditing page, click on the "Advanced Properties" and check the Retention (Days) set.</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step4.png"/>
6. Repeat steps number 2 - 5 to ensures that SQL Server Auditing retention policy is set to greater than 90 days.</br>
7. Navigate to "SQL server", select the corresponding "SQL server", scroll down the left navigation panel and choose "Auditing" under the Security.</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step7.png"/>
8. On the "SQL server - Auditing" page, scroll down, click on the "Advanced Properties" and set the Retention (Days) to 90 and click on the Save button at the top to make the changes.</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step8.png"/>
9. Repeat steps number 7 - 8 to ensure that the storage account retention policy for each SQL server is set to greater than 90 days. </br>



