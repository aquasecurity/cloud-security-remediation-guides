[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Servers / Audit Retention Policy

## Quick Info

| | |
|-|-|
| **Plugin Title** | Audit Retention Policy |
| **Cloud** | AZURE |
| **Category** | SQL Servers |
| **Description** | Ensures that SQL Server Auditing retention policy is set to greater than 90 days |
| **More Info** | Enabling SQL Server Auditing ensures that all activities are being logged properly, including potentially-malicious activity. Having a long retention policy ensures that all logs are kept for auditing and legal purposes. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/sql-database/sql-database-auditing |
| **Recommended Action** | Ensure that the storage account retention policy for each SQL server is set to greater than 90 days. |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for SQL servers. </br> <img src="/resources/azure/sqlservers/audit-retention-policy/step2.png"/>
3. On the "SQL server" page, select the SQL server that needs to be examine.</br> <img src="/resources/azure/sqlservers/audit-retention-policy/step3.png"/>
4. On the selected "SQL server" page, scroll down the left navigation panel and select "Auditing" under the "Security."</br> <img src="/resources/azure/sqlservers/audit-retention-policy/step4.png"/>
5. On the "Auditing configuration page", select the "Storage/Log Analytics/Event Hub" depending on what is used.</br> <img src="/resources/azure/sqlservers/audit-retention-policy/step5.png"/>
6. On the "Storage settings" page, check the number of "Retention(days)". If this value is set to less than 90 then the selected "SQL server" don't have a proper long retention policy.</br> <img src="/resources/azure/sqlservers/audit-retention-policy/step6.png"/>
7. Repeat steps number 2 - 6 to verify other "SQL servers" in the account.</br>
8. Navigate to "SQL servers", on the "SQL servers" page select the "SQL server", scroll down the left navigation panel and choose "Auditing" under the "Security."</br> <img src="/resources/azure/sqlservers/audit-retention-policy/step8.png"/>
9. On the "Auditing configuration page", select the "Storage/Log Analytics/Event Hub" depending on what is used.</br> <img src="/resources/azure/sqlservers/audit-retention-policy/step9.png"/>
10. On the "Storage settings" page, set the "Retention(days)" to 90 or more and save the changes.</br> <img src="/resources/azure/sqlservers/audit-retention-policy/step10.png"/>
11. Repeat steps number 8 - 10 to ensure that the storage account retention policy for each SQL server is set to greater than 90 days.</br>
