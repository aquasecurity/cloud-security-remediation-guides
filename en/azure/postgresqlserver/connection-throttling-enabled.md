[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / PostgreSQL Server / Connection Throttling Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Connection Throttling Enabled |
| **Cloud** | AZURE |
| **Category** | PostgreSQL Server |
| **Description** | Ensures connection throttling is enabled for PostgreSQL servers |
| **More Info** | Connection throttling slows the amount of query and error logs sent by the server from the same IP address, limiting DoS attacks or the slowing down of servers due to excessive legitimate user logs. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/postgresql/howto-configure-server-parameters-using-portal |
| **Recommended Action** | Ensure the server parameters for each PostgreSQL server have the connection_throttling setting enabled. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for PostgreSQL. </br> <img src="/resources/azure/postgresqlserver/connection-throttling-enabled/step2.png"/>
3. On the "Azure Database for PostgreSQL servers" page, select the database by clicking on the "Name" as a link that needs to be examine.</br> <img src="/resources/azure/postgresqlserver/connection-throttling-enabled/step3.png"/>
4. Scroll down the left navigation panel and choose "Server parameters" under "Settings."</br> <img src="/resources/azure/postgresqlserver/connection-throttling-enabled/step4.png"/>
5. On the "Server parameters" page, search for "connection_throttling" paramter using the "Search for filter item search box." If the value is set to "OFF" then the connection throttling is not enabled for PostgreSQL servers.</br> <img src="/resources/azure/postgresqlserver/connection-throttling-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "PostgreSQL" databases in the account.</br>
7. Navigate to "PostgreSQL", select the database by clicking on the "Name" and choose "Server parameters" under "Settings" from the left navigation panel.</br> <img src="/resources/azure/postgresqlserver/connection-throttling-enabled/step7.png"/>
8. On "Server Parameter" page, search for "connection_throttling" paramter using the "Search for filter item search box" and enable it by selecting "ON" from the toggle configuration button.</br> <img src="/resources/azure/postgresqlserver/connection-throttling-enabled/step8.png"/>
9. Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/postgresqlserver/connection-throttling-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to ensure the server parameters for each PostgreSQL server have the connection_throttling setting enabled.</br>
