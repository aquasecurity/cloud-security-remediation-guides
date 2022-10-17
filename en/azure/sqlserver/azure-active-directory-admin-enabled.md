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
2. Select the "Search resources, services, and docs" option at the top and search for "SQL Server".</br> <img src="/resources/azure/sqlserver/azure-active-directory-admin-enabled/step2.png"/>
3. On the "SQL server" page, select the SQL server by clicking on the "Name" as a link.</br> <img src="/resources/azure/sqlserver/azure-active-directory-admin-enabled/step3.png"/>
4. On the "SQL server" Overview page, scroll down and select the "Azure Active Directory" under the Settings.</br> <img src="/resources/azure/sqlserver/azure-active-directory-admin-enabled/step4.png"/>
5. In the "Azure Active Directory" page, if "No Active Directory admin" is showing then the AD admin is not enabled on all SQL servers.</br> <img src="/resources/azure/sqlserver/azure-active-directory-admin-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to check other SQL servers in the account.</br>
7. Navigate to "SQL server", select the corresponding "SQL server", scroll down the left navigation panel and choose "Azure Active Directory" under the Settings.</br> <img src="/resources/azure/sqlserver/azure-active-directory-admin-enabled/step7.png"/>
8. On the "SQL server - Azure Active Directory" page, click on the "Set Admin" button at the top.</br> <img src="/resources/azure/sqlserver/azure-active-directory-admin-enabled/step8.png"/>
9. Select the "Azure Active Directory - Admin" as per the requirement and click on the "Select" button.</br> <img src="/resources/azure/sqlserver/azure-active-directory-admin-enabled/step9.png"/>
10. Click on the "Save" button to make the changes.</br> <img src="/resources/azure/sqlserver/azure-active-directory-admin-enabled/step10.png"/>
11. Repeat steps number 6 - 10 to ensure Azure Active Directory admin is enabled on all SQL servers.</br>



