[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / PostgreSQL Server / Log Retention Period

## Quick Info

| | |
|-|-|
| **Plugin Title** | Log Retention Period |
| **Cloud** | AZURE |
| **Category** | PostgreSQL Server |
| **Description** | Ensures logs are configured to be retained for 4 or more days for PostgreSQL servers |
| **More Info** | Having a long log retention policy ensures that all critical logs are stored for long enough to access and view in case of a security incident. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/postgresql/howto-configure-server-parameters-using-portal |
| **Recommended Action** | Ensure the server parameters for each PostgreSQL server have the log_retention_days setting set to 4 or more days. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for PostgreSQL. </br> <img src="/resources/azure/postgresqlserver/log-retention-period/step2.png"/>
3. On the "Azure Database for PostgreSQL servers" page, select the database by clicking on the "Name" as a link that needs to be examine.</br> <img src="/resources/azure/postgresqlserver/log-retention-period/step3.png"/>
4. Scroll down the left navigation panel and choose "Server parameters" under "Settings."</br> <img src="/resources/azure/postgresqlserver/log-retention-period/step4.png"/>
5. On the "Server parameters" page, search for "log_retention_days" paramter using the "Search for filter item search box." If the value is set to less than "3 days" then the "log_retention_days" is not as per best practices for PostgreSQL servers.</br> <img src="/resources/azure/postgresqlserver/log-retention-period/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "PostgreSQL" databases in the account.</br>
7. Navigate to "PostgreSQL", select the database by clicking on the "Name" and choose "Server parameters" under "Settings" from the left navigation panel.</br> <img src="/resources/azure/postgresqlserver/log-retention-period/step7.png"/>
8. On "Server Parameter" page, search for "log_retention_days" paramter using the "Search for filter item search box" and set the "log_retention_days" more than "4 days."</br> <img src="/resources/azure/postgresqlserver/log-retention-period/step8.png"/>
9. Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/postgresqlserver/log-retention-period/step9.png"/>
10. Repeat steps number 7 - 9 to ensure the server parameters for each PostgreSQL server have the log_retention_days setting set to 4 or more days.</br>
