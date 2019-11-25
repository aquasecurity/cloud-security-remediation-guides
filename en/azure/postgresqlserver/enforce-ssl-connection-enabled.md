[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / PostgreSQL Server / Enforce SSL Connection Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Enforce SSL Connection Enabled |
| **Cloud** | AZURE |
| **Category** | PostgreSQL Server |
| **Description** | Ensures SSL connections are enforced on PostgreSQL Servers |
| **More Info** | SSL prevents infiltration attacks by encrypting the data stream between the server and application. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/postgresql/concepts-ssl-connection-security |
| **Recommended Action** | Ensure the connection security settings of each PostgreSQL server are configured to enforce SSL connections. |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for PostgreSQL. </br> <img src="/resources/azure/postgresqlserver/enforce-ssl-connection-enabled/step2.png"/>
3. On the "Azure Database for PostgreSQL servers" page, select the database by clicking on the "Name" as a link that needs to be examine.</br> <img src="/resources/azure/postgresqlserver/enforce-ssl-connection-enabled/step3.png"/>
4. Scroll down the left navigation panel and choose "Connection Security" under "Settings."</br> <img src="/resources/azure/postgresqlserver/enforce-ssl-connection-enabled/step4.png"/>
5. On the "Connection Security" page, scroll down the page and look for "Enforce SSL connection" under "SSL settings". If it's "DISABLED" then SSL connections are not enforced on PostgreSQL Servers. </br> <img src="/resources/azure/postgresqlserver/enforce-ssl-connection-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "PostgreSQL" databases for SSL connection in the account.</br>
7. Navigate to "PostgreSQL", select the database by clicking on the "Name" and choose "Connection Security" under "Settings" from the left navigation panel.</br> <img src="/resources/azure/postgresqlserver/enforce-ssl-connection-enabled/step7.png"/>
8. On "Connection Security" page, scroll down and under "SSL Settings", click on the "ENABLED" toggle button next to the "Enforce SSL connection." </br> <img src="/resources/azure/postgresqlserver/enforce-ssl-connection-enabled/step8.png"/>
9. Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/postgresqlserver/enforce-ssl-connection-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to ensure the connection security settings of each PostgreSQL server are configured to enforce SSL connections.</br>
