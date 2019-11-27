[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Servers / Server Auditing Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Server Auditing Enabled |
| **Cloud** | AZURE |
| **Category** | SQL Servers |
| **Description** | Ensures that SQL Server Auditing is enabled for SQL servers |
| **More Info** | Enabling SQL Server Auditing ensures that all activities are being logged properly, including potentially-malicious activity. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/sql-database/sql-database-auditing |
| **Recommended Action** | Ensure that auditing is enabled for each SQL server. |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for SQL servers. </br> <img src="/resources/azure/sqlservers/server-auditing-enabled/step2.png"/>
3. On the "SQL server" page, select the SQL server that needs to be examine.</br><img src="/resources/azure/sqlservers/server-auditing-enabled/step3.png"/>
4. On the selected "SQL server" page, scroll down the left navigation panel and select "Auditing" under the "Security."</br> <img src="/resources/azure/sqlservers/server-auditing-enabled/step4.png"/>
5. On the "Auditing configuration page", verify the "Auditing" staus. If it's set to "OFF" then "SQL Server Auditing" is not enabled for the selected "SQL server." </br> <img src="/resources/azure/sqlservers/server-auditing-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "SQL servers" in the account.</br>
7. Navigate to "SQL servers", on the "SQL servers" page select the "SQL server", scroll down the left navigation panel and choose "Auditing" under the "Security."</br> <img src="/resources/azure/sqlservers/server-auditing-enabled/step7.png"/>
8. On the "Auditing configuration page", click on the "ON" option next to "Auditing" and "Save" the changes. </br> <img src="/resources/azure/sqlservers/server-auditing-enabled/step8.png"/>
9. Repeat steps number 7 - 8 to ensure that auditing is enabled for each SQL server.</br>
