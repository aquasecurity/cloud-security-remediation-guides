[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Databases / SQL DB Multiple AZ

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQL DB Multiple AZ |
| **Cloud** | AZURE |
| **Category** | SQL Databases |
| **Description** | Ensures that SQL Database instances are created to be cross-AZ for high availability |
| **More Info** | Creating SQL Database instances in a single availability zone creates a single point of failure for all systems relying on that database. All SQL Database instances should be created in multiple availability zones to ensure proper failover. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/sql-database/sql-database-high-availability#zone-redundant-configuration |
| **Recommended Action** | Ensure that each SQL Database is configured to be zone redundant. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "SQL databases". </br> <img src="/resources/azure/sqldatabases/db-restorable/step2.png"/>
3. On the "SQL database" page, click on the "Cloud shell" icon at the top next to the search bar as "Availability Zones" cannot be checked from Azure "UI Console".</br> <img src="/resources/azure/sqldatabases/db-restorable/step3.png"/>
4. In the box that opens at the bottom, select "PowerShell".</br> <img src="/resources/azure/sqldatabases/db-restorable/step4.png"/>
5. In the next screen, select the desired Azure Subscription & click on "Create storage" button.</br> <img src="/resources/azure/sqldatabases/db-restorable/step5.png"/>
6. Run "Get-AzSqlServer" PowerShell command in the PowerShell prompt, to list all the "SQL servers" in the selected subscription. Note the "ResourceGroupName" and "ServerName" of the desired SQL server.</br> <img src="/resources/azure/sqldatabases/db-restorable/step6.png"/>
7. Run "Get-AzSqlDatabase -ResourceGroupName your_resource_groupname -ServerName your_server_name -DatabaseName your_DB_Name" PowerShell command.</br> <img src="/resources/azure/sqldatabases/db-restorable/step7.png"/>
8. If the value of property "ZoneReduntant" is "false" in the result then the database is not zone reduntant.</br> <img src="/resources/azure/sqldatabases/db-restorable/step8.png"/>
9. If the value of ZoneReduntant is False then we need to restore the affected Database with a minimum of "Premium" grade database.
10. On the Azure UI Dashboard, goto to the configuration of the affected database and click on "Restore" button at the top.</br> <img src="/resources/azure/sqldatabases/db-restorable/step8.png"/>
11. On the "Create SQL Database - Restore database" page, select the "Earliest restore point" and click on "Configure database" next to "Compute + storage".</br> <img src="/resources/azure/sqldatabases/db-restorable/step11.png"/>
12. On the Configure page, select "Premium" or higher Service tier type in the "Service tier" dropdown.Then select "yes" for "Would you like to make this database zone redundant?" and click "Apply" button at the bottom.</br> <img src="/resources/azure/sqldatabases/db-restorable/step12.png"/>
13. Now click "Review + create" and "Create" on the "Create SQL Database - Restore database" page to complete the restoration.
14. Once the restoration is complete, on Azure PowerShell run the command "Get-AzSqlDatabase -ResourceGroupName your_resource_groupname -ServerName your_server_name -DatabaseName your_DB_Name" to verify that zone reduntant property is now "True".
15. Repeat steps 3 - 14 for all other SQL databases to make them zone redundant.
