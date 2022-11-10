[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / MySQL Server / Enforce MySQL SSL Connection

## Quick Info

| | |
|-|-|
| **Plugin Title** | Enforce MySQL SSL Connection |
| **Cloud** | AZURE |
| **Category** | MySQL Server |
| **Description** | Ensures SSL connection is enforced on MySQL servers |
| **More Info** | MySQL servers should be set to use SSL for data transmission to ensure all data is encrypted in transit. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/mysql/concepts-ssl-connection-security |
| **Recommended Action** | Ensure the connection security of each Azure Database for MySQL is configured to enforce SSL connections. |

## Detailed Remediation Steps

[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / MySQLServer / Enfore MySQL SSL Connection

## Quick Info

| | |
|-|-|
| **Plugin Title** | Enforce MySQL SSL Connection |
| **Cloud** | AZURE |
| **Category** | MySQL Server |
| **Description** | Ensures SSL connection is enforced on MySQL servers |
| **More Info** | MySQL servers should be set to use SSL for data transmission to ensure all data is encrypted in transit. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/mysql/concepts-ssl-connection-security |
| **Recommended Action** | Ensure the connection security of each Azure Database for MySQL is configured to enforce SSL connections. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. In search bar at the top search for Mysql and select "Azure Database for MySQL Servers". </br> <img src="/resources/azure/mysqlserver/enforce-mysql-ssl-connection/step2.png"/>
3. Select a server by clicking on the "Name" link to load the configuration pane.</br> <img src="/resources/azure/mysqlserver/enforce-mysql-ssl-connection/step3.png"/>
4. On the configuration pane that opens, scroll down the left navigation panel and choose the "Connection security" option. </br>  <img src="/resources/azure/mysqlserver/enforce-mysql-ssl-connection/step4.png"/>
5. On the "Connection security" pane that opens, scroll down to "SSL settings". If "Enforce SSL connection" is set to "Disabled" then insecure traffic is allowed in the server. This is a security risk and should be disabled.</br>  <img src="/resources/azure/mysqlserver/enforce-mysql-ssl-connection/step5.png"/>
6. Click "Enabled" next to "Enforce SSL connection" to enable SSL. Under "TLS setting" select the highest version for "Minimum TLS version" (1.2) as of this writing.</br>  <img src="/resources/azure/mysqlserver/enforce-mysql-ssl-connection/step6.png"/>
7. Click on "Save" button at the top to complete the changes.</br>  <img src="/resources/azure/mysqlserver/enforce-mysql-ssl-connection/step7.png"/>
8. Repeat step number 3 - 7 to check all other MySQL servers for secure traffic.

