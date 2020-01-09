[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Server / SQL Server Public Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQL Server Public Access |
| **Cloud** | AZURE |
| **Category** | SQL Server |
| **Description** | Ensures that SQL Servers do not allow public access |
| **More Info** | Unless there is a specific business requirement, SQL Server instances should not have a public endpoint and should only be accessed from within a VNET. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/sql-database/sql-database-security-overview/ |
| **Recommended Action** | Ensure that the firewall of each SQL Server is configured to prohibit traffic from the public 0.0.0.0 global IP address. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for SQL servers. </br> <img src="/resources/azure/sqlserver/sql-server-public-access/step2.png"/>
3. On the "SQL server" page, select the SQL server that needs to be examined. </br> <img src="/resources/azure/sqlserver/sql-server-public-access/step3.png"/>
4. On the selected "SQL server" page, scroll down the left navigation panel and select " Firewalls and virtual networks" under the "Security" column.</br> <img src="/resources/azure/sqlserver/sql-server-public-access/step4.png"/>
5. On the "Firewalls and virtual networks" page, if "Allow Azure services and resources to access this server" is "ON" then the selected "SQL server" allow public access.</br> <img src="/resources/azure/sqlserver/sql-server-public-access/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "SQL servers" in the account.</br>
7. Navigate to "SQL servers", on the "SQL servers" page select the "SQL server", scroll down the left navigation panel and choose "Firewalls and virtual networks" under the "Security."</br> <img src="/resources/azure/sqlserver/sql-server-public-access/step7.png"/>
8. On the "Firewalls and virtual networks" page, click on the "OFF" option next to the "Allow Azure services and resources to access this server" and "Save" the changes.</br> <img src="/resources/azure/sqlserver/sql-server-public-access/step8.png"/>
9. If no "VNET" is configured, scroll down the page and click on the "Add existing virtual network".</br> <img src="/resources/azure/sqlserver/sql-server-public-access/step9.png"/>
10. On the "Create/Update" page, select the "Subscription", "Virtual network", "Subnet name" and click on "OK" at the bottom of the page.</br> <img src="/resources/azure/sqlserver/sql-server-public-access/step10.png"/>
11. Click on the "Save" button to make the changes.</br> <img src="/resources/azure/sqlserver/sql-server-public-access/step11.png"/>
12. Repeat steps number 7 - 11 to ensure that the firewall of each SQL Server is configured to prohibit traffic from the public 0.0.0.0 global IP address.</br>
