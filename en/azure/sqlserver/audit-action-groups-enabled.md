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

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "SQL servers". </br> <img src="/resources/azure/sqlserver/audit-action-groups-enabled/step2.png"/>
3. On the "SQL server" page, click on the "Cloud shell" icon at the top next to the search bar as "Audit Action Groups Enabled" cannot be checked from Azure "UI Console".</br> <img src="/resources/azure/sqlserver/audit-action-groups-enabled/step3.png"/>
4. In the box that opens at the bottom, select "PowerShell".</br> <img src="/resources/azure/sqlserver/audit-action-groups-enabled/step3.png"/>
5. In the next screen, select the desired Azure Subscription & click on "Create storage" button.</br> <img src="/resources/azure/sqlserver/audit-action-groups-enabled/step5.png"/>
6. Run "Get-AzSqlServer" PowerShell command in the PowerShell prompt, to list all the "SQL servers" in the selected subscription. Note the "ResourceGroupName" and "ServerName" of the desired SQL server. </br> <img src="/resources/azure/sqlserver/audit-action-groups-enabled/step6.png"/>
7. Run "Get-AzSqlServerAudit -ResourceGroupName your_resource_group_name -ServerName your_server_name" PowerShell command.</br> <img src="/resources/azure/sqlserver/audit-action-groups-enabled/step7.png"/>
8. In the result if the "AuditActionGroup" property value is {}(empty) then Audit Action Groups are not enabled. </br> <img src="/resources/azure/sqlserver/audit-action-groups-enabled/step8.png"/> 
9. Run "Set-AzSqlServerAudit -ServerName your_server_name -ResourceGroupName your_resource_group_name -AuditActionGroup SUCCESSFUL_DATABASE_AUTHENTICATION_GROUP, FAILED_DATABASE_AUTHENTICATION_GROUP, BATCH_COMPLETED_GROUP". </br> <img src="/resources/azure/sqlserver/audit-action-groups-enabled/step9.png"/>
10. Run "Get-AzSqlServerAudit -ResourceGroupName your_resource_group_name -ServerName your_server_name" PowerShell command to verify that "AuditActionGroup" property value is not {}(empty).
11. Repeat step number 3-10 to check and configure SQL Server Audit Groups for all other SQL servers.</br>
