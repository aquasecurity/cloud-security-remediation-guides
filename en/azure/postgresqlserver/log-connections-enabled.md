[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / PostgreSQL Server / Log Connections Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Log Connections Enabled |
| **Cloud** | AZURE |
| **Category** | PostgreSQL Server |
| **Description** | Ensures connection logs are enabled for PostgreSQL servers |
| **More Info** | Connection logs ensure all attempted and successful connections to the server are logged. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/postgresql/howto-configure-server-parameters-using-portal |
| **Recommended Action** | Ensure the server parameters for each PostgreSQL server have the log_connections setting enabled. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for PostgreSQL. </br> <img src="/resources/azure/postgresqlserver/log-connections-enabled/step2.png"/>
3. On the "Azure Database for PostgreSQL servers" page, select the database by clicking on the "Name" as a link that needs to be examined.</br> <img src="/resources/azure/postgresqlserver/log-connections-enabled/step3.png"/>
4. Scroll down the left navigation panel and choose "Server parameters" under "Settings."</br> <img src="/resources/azure/postgresqlserver/log-connections-enabled/step4.png"/>
5. On the "Server parameters" page, search for "log_connections" paramter using the "Search for filter item search box." If the value is set to "OFF" then the "Log Connections" are not enabled for PostgreSQL servers. This is against Azure best practices.</br> <img src="/resources/azure/postgresqlserver/log-connections-enabled/step5.png"/>
6. To enable "log_connections" select "ON" from the toggle configuration button.</br> <img src="/resources/azure/postgresqlserver/log-connections-enabled/step6.png"/>
7. Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/postgresqlserver/log-connections-enabled/step7.png"/>
8. Repeat step number 3 - 7 to ensure the server parameters for each PostgreSQL server have the log_connections setting enabled.</br>
