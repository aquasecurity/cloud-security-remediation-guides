[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / PostgreSQL Server / PostgreSQL Server Access to Azure Services Disabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | PostgreSQL Server Access to Azure Services Disabled |
| **Cloud** | AZURE |
| **Category** | PostgreSQL Server |
| **Description** | Ensure that Allow access to Azure services for PostgreSQL Database Server is disabled. |
| **More Info** | If access from Azure services is enabled, the server\'s firewall will accept connections from all Azure resources, including resources not in your subscription. This is usually not a desired configuration. Instead, set up firewall rules to allow access from specific network ranges or VNET rules to allow access from specific virtual networks. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/postgresql/flexible-server/concepts-firewall-rules |
| **Recommended Action** | Disable network access to the public for PostgreSQL database servers. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for PostgreSQL. </br> <img src="/resources/azure/postgresqlserver/postgresql-public-access-disabled/step2.png"/>
3. On the "Azure Database for PostgreSQL servers" page, select the database by clicking on the "Name" as a link that needs to be examined.</br> <img src="/resources/azure/postgresqlserver/postgresql-public-access-disabled/step3.png"/>
4. Click on "Networking" from navigation panel on the left under settings section.</br> <img src="/resources/azure/postgresqlserver/postgresql-public-access-disabled/step4.png"/>
5. On the "Networking" page, under the firewall rule uncheck the "Allow public access from any Azure service" option and Click "Save" on top navigation panel.</br> <img src="/resources/azure/postgresqlserver/postgresql-public-access-disabled/step5.png"/>



