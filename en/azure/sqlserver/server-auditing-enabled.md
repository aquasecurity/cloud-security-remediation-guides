[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Server / Server Auditing Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Server Auditing Enabled |
| **Cloud** | AZURE |
| **Category** | SQL Server |
| **Description** | Ensures that SQL Server Auditing is enabled for SQL servers |
| **More Info** | Enabling SQL Server Auditing ensures that all activities are being logged properly, including potentially-malicious activity. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/sql-database/sql-database-auditing |
| **Recommended Action** | Ensure that auditing is enabled for each SQL server. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "SQL Server".</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step2.png"/>
3. On the "SQL server" page, select the SQL server by clicking on the "Name" as a link.</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step3.png"/>
4. On the "SQL server" Overview page, scroll down and select the "Auditing" under the Security.</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step4.png"/>
5. On the "SQL server" Auditing page, if Azure SQL Auditing is not enabled then the all activities are not being logged properly, including potentially-malicious activity.</br>  <img src="/resources/azure/sqlserver/server-auditing-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to check other SQL servers in the account.</br>
7. Navigate to "SQL server", select the corresponding "SQL server", scroll down the left navigation panel and choose "Auditing" under the Security.</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step7.png"/>
8. On the "SQL server - Auditing" page, click on the toggle button next to the "Enable Azure SQL Auditing".</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step8.png"/>
9. Select the "Audit log destination" from the options as per the requirement, select the "Subscription" and "Storage Account" if in the case "Audit log destination" is Storage account.</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step9.png"/>
10. Click on the "Save" button to make the changes.</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step10.png"/>
11. Repeat steps number 7 - 10 to ensure that auditing is enabled for each SQL server.</br>



