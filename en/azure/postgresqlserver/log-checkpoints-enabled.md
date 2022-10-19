[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / PostgreSQL Server / Log Checkpoints Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Log Checkpoints Enabled |
| **Cloud** | AZURE |
| **Category** | PostgreSQL Server |
| **Description** | Ensures log checkpoints are enabled for PostgreSQL servers |
| **More Info** | Log checkpoints logs queries and errors that arise in the server, enabling faster detection of incidents. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/postgresql/howto-configure-server-parameters-using-portal |
| **Recommended Action** | Ensure the server parameters for each PostgreSQL server have the log_checkpoints setting enabled. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for PostgreSQL. </br> <img src="/resources/azure/postgresqlserver/log-checkpoints-enabled/step2.png"/>
3. On the "Azure Database for PostgreSQL servers" page, select the database by clicking on the "Name" as a link that needs to be examined.</br> <img src="/resources/azure/postgresqlserver/log-checkpoints-enabled/step3.png"/>
4. Scroll down the left navigation panel and choose "Server parameters" under "Settings."</br> <img src="/resources/azure/postgresqlserver/log-checkpoints-enabled/step4.png"/>
5. On the "Server parameters" page, search for "log_checkpoints" paramter using the "Search for filter item search box." If the value is set to "OFF" then the log checkpoints are not enabled for PostgreSQL servers. This is against Azure best practices.</br> <img src="/resources/azure/postgresqlserver/log-checkpoints-enabled/step5.png"/>
6. To enable "log_checkpoints" select "ON" from the toggle configuration button.</br> <img src="/resources/azure/postgresqlserver/log-checkpoints-enabled/step6.png"/>
7. Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/postgresqlserver/log-checkpoints-enabled/step7.png"/>
8. Repeat step number 3 - 7 to ensure the server parameters for each PostgreSQL server have the log_checkpoints setting enabled.</br>
