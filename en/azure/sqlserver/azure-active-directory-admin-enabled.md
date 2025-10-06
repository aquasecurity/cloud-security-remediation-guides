[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Server / Azure Entra ID Admin Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Azure Entra ID Admin Enabled |
| **Cloud** | AZURE |
| **Category** | SQL Server |
| **Description** | Ensures that Entra ID admin is enabled on all SQL servers. |
| **More Info** | Enabling Entra ID admin allows users to manage account admins in a central location, allowing key rotation and permission management to be managed in one location for all servers and databases. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/sql-database/sql-database-aad-authentication-configure |
| **Recommended Action** | Ensure Azure Entra ID admin is enabled on all SQL servers. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "SQL servers". </br> <img src="/resources/azure/sqlserver/azure-active-directory-admin-enabled/step2.png"/>
3. On the "SQL server" page, select the SQL server that needs to be examined. </br> <img src="/resources/azure/sqlserver/azure-active-directory-admin-enabled/step3.png"/>
4. On the selected "SQL server" page, scroll down the left navigation panel and select "Azure Entra ID" under "Settings".</br> <img src="/resources/azure/sqlserver/azure-active-directory-admin-enabled/step4.png"/>
5. On the "Azure Entra ID" page, if "Admin name" under "Azure Entra ID admin" states "No Entra ID admin" then Azure Entra ID admin is not enabled on selected SQL server. </br> <img src="/resources/azure/sqlserver/azure-active-directory-admin-enabled/step5.png"/>
6. To enable Azure Entra ID admin click on "Set admin" at the top. </br> <img src="/resources/azure/sqlserver/azure-active-directory-admin-enabled/step6.png"/>
7. On the Azure Entra ID pop up, search for the desired admin name and select the user from the results and click "Select" button at the bottom of the page.</br> <img src="/resources/azure/sqlserver/azure-active-directory-admin-enabled/step7.png"/>
8. Click the "Save" button at the top to make the changes.</br> <img src="/resources/azure/sqlserver/azure-active-directory-admin-enabled/step8.png"/>
9. Repeat steps 3 - 8 to ensure Azure Entra ID admin is enabled on all SQL servers.
