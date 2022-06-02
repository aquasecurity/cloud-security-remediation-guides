[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / PostgreSQL Server / Enforce PostgreSQL SSL Connection

## Quick Info

| | |
|-|-|
| **Plugin Title** | Enforce PostgreSQL SSL Connection |
| **Cloud** | AZURE |
| **Category** | PostgreSQL Server |
| **Description** | Ensures SSL connections are enforced on PostgreSQL Servers |
| **More Info** | SSL prevents infiltration attacks by encrypting the data stream between the server and application. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/postgresql/concepts-ssl-connection-security |
| **Recommended Action** | Ensure the connection security settings of each PostgreSQL server are configured to enforce SSL connections. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for PostgreSQL. </br> <img src="/resources/azure/postgresqlserver/connection-throttling-enabled/step2.png"/>
3. On the "Azure Database for PostgreSQL servers" page, select the database by clicking on the "Name" as a link that needs to be examine.</br> <img src="/resources/azure/postgresqlserver/connection-throttling-enabled/step3.png"/>
4. Scroll down the left navigation panel and choose "Connection Security" under "Settings."</br> <img src="/resources/azure/postgresqlserver/connection-throttling-enabled/step4.png"/>
5. On the "Connection Security" page, search for "SSL settings". If the Enforce SSL connection is set to "DISABLED" this is a security risk as data is transmitted unencrypted. This is against azure best practices.</br> <img src="/resources/azure/postgresqlserver/connection-throttling-enabled/step5.png"/>
6. To Enable the "SSL Connection" select "ENABLED" from the toggle configuration button. In the "TLS setting" select the highest version "1.2" as of now.</br> <img src="/resources/azure/postgresqlserver/connection-throttling-enabled/step6.png"/>
7. Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/postgresqlserver/connection-throttling-enabled/step7.png"/>
8. Repeat steps number 3 - 7 to ensure the server parameters for each PostgreSQL server have the connection_throttling setting enabled.</br>





