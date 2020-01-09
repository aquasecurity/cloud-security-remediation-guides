[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Server / Audit Action Groups Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Audit Action Groups Enabled |
| **Cloud** | AZURE |
| **Category** | SQL Server |
| **Description** | Ensures that SQL Server Audit Action and Groups is configured properly |
| **More Info** | SQL Server Audit Action and Groups should be configured to at least include SUCCESSFUL_DATABASE_AUTHENTICATION_GROUP, FAILED_DATABASE_AUTHENTICATION_GROUP and BATCH_COMPLETED_GROUP. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/sql-database/sql-database-auditing |
| **Recommended Action** | If SQL Server Audit Action and Groups is not configured properly when enabling Auditing, these settings must be configured in Powershell. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for SQL servers. </br> <img src="/resources/azure/sqlserver/audit-action-groups-enabled/step2.png"/>
3. On the "SQL server" page, click on the "Cloud shell" button at the top to access "Power Shell" as "Audit Action Groups Enabled" cannot be checked from A"zure UI Console".</br> <img src="/resources/azure/sqlserver/audit-action-groups-enabled/step3.png"/>
4. Run Get-AzSqlServer PowerShell command, to list all the "SQL servers" in the selected subscription.</br> <img src="/resources/azure/sqlserver/audit-action-groups-enabled/step4.png"/>
5. Run Get-AzSqlServerAuditing PowerShell command with name of "SQL server" name that needs to be examine along with identifier parameter and custom query filters.</br> <img src="/resources/azure/sqlserver/audit-action-groups-enabled/step5.png"/>
6. The above command will return name of the each action group which are enabled and if it's showing "FAILED_DATABASE_AUTHENTICATION_GROUP" then there is no "Audit Action Groups Enabled."<br> <img src="/resources/azure/sqlserver/audit-action-groups-enabled/step6.png"/>
7. Repeat steps number 2 - 6 to verify other "SQL server" in different Azure accounts.</br> 
8. Run Set-AzSqlServerAuditing PowerShell along with "Server name", "Resource group" and "Retention days." Command can use like "Set-AzSqlServerAuditing -State Enabled -ServerName "cc-pr" -ResourceGroupName "test-noc26" -StorageAccountName "abinnf890" -AuditActionGroupSet-AzSqlServerAuditing -State Enabled -ServerName "testnov26" -ResourceGroupName "test-noc26" -StorageAccountName "abinnf890" -AuditActionGroup "SUCCESSFUL_DATABASE_AUTHENTICATION_GROUP", "FAILED_DATABASE_AUTHENTICATION_GROUP", "BATCH_COMPLETED_GROUP" -RetentionInDays 90". </br> <img src="/resources/azure/sqlserver/audit-action-groups-enabled/step8.png"/>
9. Repeat step number 8 to configure SQL Server Audit Action and Groups.</br>
