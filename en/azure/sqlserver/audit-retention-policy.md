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
2. Select the "Search resources, services, and docs" option at the top and search for "SQL servers". </br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step2.png"/>
3. On the "SQL server" page, select the SQL server that needs to be examined. </br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step3.png"/>
4. On the selected "SQL server" page, scroll down the left navigation panel and select "Auditing" under "Security".</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step4.png"/>
5. On the "Auditing" page, if "Azure SQL Auditing" and "Auditing of Microsoft support operations" is disabled then SQL Server Auditing for all activities are not being logged properly.</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step5.png"/>
6. To ensure that auditing is enabled for each SQL server, go to "Auditing" page and turn the toggle "ON" for "Enable Azure SQL Auditing" and under "Audit log destination" checkmark "Storage", "Log Analytics", "Event hub" selecting the "Subscription" and "Storage end points" under each section.</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step6.png"/>
7. Turn the toggle "ON" for "Auditing of Microsoft support operations" and under "Audit log destination" checkmark "Storage", "Log Analytics", "Event hub" selecting the "Subscription" and "Storage end points" under each section.</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step7.png"/>
8. Click on "Save" at the top to make the necessary changes.</br> <img src="/resources/azure/sqlserver/server-auditing-enabled/step8.png"/>
9. Repeat steps 3-8 to ensure that auditing is enabled for each SQL server.



