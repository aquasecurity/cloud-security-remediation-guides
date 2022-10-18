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
2. Select the "Search resources, services, and docs" option at the top and search for "SQL servers". </br> <img src="/resources/azure/sqlserver/audit-retention-policy/step2.png"/>
3. On the "SQL server" page, select the SQL server that needs to be examined. </br> <img src="/resources/azure/sqlserver/audit-retention-policy/step3.png"/>
4. On the selected "SQL server" page, scroll down the left navigation panel and select "Auditing" under "Security".</br> <img src="/resources/azure/sqlserver/audit-retention-policy/step4.png"/>
5. On the "Auditing" page, scroll down to "Audit log destination" and click on Advanced properties" under "Storage". </br> <img src="/resources/azure/sqlserver/audit-retention-policy/step5.png"/>
6. If the Retention (Days)is set to zero then audit logs are not being retained.</br> <img src="/resources/azure/sqlserver/audit-retention-policy/step6.png"/>
7. To ensure that the storage account retention policy for each SQL server is set to greater than 90 days, drag the slider or type 365 in the text box.</br> <img src="/resources/azure/sqlserver/audit-retention-policy/step7.png"/>
8. Click on "Save" at the top to make the necessary changes.</br> <img src="/resources/azure/sqlserver/audit-retention-policy/step8.png"/>
9. Repeat steps 3-8 to ensure that SQL Server Auditing retention policy is set to greater than 90 days.
