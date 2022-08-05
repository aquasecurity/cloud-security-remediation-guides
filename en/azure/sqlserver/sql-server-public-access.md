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

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for SQL servers. </br> <img src="/resources/azure/sqlserver/sql-server-public-access/step2.png"/>
3. On the "SQL server" page, select the SQL server that needs to be examined. </br> <img src="/resources/azure/sqlserver/sql-server-public-access/step3.png"/>
4. On the selected "SQL server" page, scroll down the left navigation panel and select "Networking" under the "Security".</br> <img src="/resources/azure/sqlserver/sql-server-public-access/step4.png"/>
5. On the "Networking" page, under "Exceptions" if "Allow Azure services and resources to access this server" is "ON" then the selected "SQL server" allows public access.</br> <img src="/resources/azure/sqlserver/sql-server-public-access/step5.png"/>
6. To disable public access, uncheck "Allow Azure services and resources to access this server" and click "save" button.</br> <img src="/resources/azure/sqlserver/sql-server-public-access/step6.png"/>
7. Under "Firewall Rules" if you see an entry for IP address "0.0.0.0" then traffic from global public IPs is allowed. </br> <img src="/resources/azure/sqlserver/sql-server-public-access/step7.png"/>
8. To diable traffic from global public IPs, remove the firewal rule with IP address "0.0.0.0" To delete it, click on the tripple dot (...) at the end and select "Delete" from the dropdown menu.</br> <img src="/resources/azure/sqlserver/sql-server-public-access/step8.png"/>
9. Click on the "Save" button to make the changes.</br> <img src="/resources/azure/sqlserver/sql-server-public-access/step11.png"/>
10. Repeat steps number 3 - 9 to ensure that the firewall of each SQL Server is configured to prohibit traffic from the public 0.0.0.0 global IP address.</br>
