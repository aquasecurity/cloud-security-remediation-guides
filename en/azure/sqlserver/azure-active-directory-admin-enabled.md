[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Server / Azure Active Directory Admin Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Azure Active Directory Admin Enabled |
| **Cloud** | AZURE |
| **Category** | SQL Server |
| **Description** | Ensures that Active Directory admin is enabled on all SQL servers. |
| **More Info** | Enabling Active Directory admin allows users to manage account admins in a central location, allowing key rotation and permission management to be managed in one location for all servers and databases. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/sql-database/sql-database-aad-authentication-configure |
| **Recommended Action** | Ensure Azure Active Directory admin is enabled on all SQL servers. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "SQL servers". </br> <img src="/resources/azure/sqlserver/send-alerts-enabled/step2.png"/>
3. On the "SQL server" page, select the SQL server that needs to be examined. </br> <img src="/resources/azure/sqlserver/send-alerts-enabled/step3.png"/>
4. On the selected "SQL server" page, scroll down the left navigation panel and select "Azure Active Directory" under "Settings".</br> <img src="/resources/azure/sqlserver/send-alerts-enabled/step4.png"/>





