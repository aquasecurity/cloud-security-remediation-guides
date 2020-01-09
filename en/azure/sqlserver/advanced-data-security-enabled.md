[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Server / Advanced Data Security Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Advanced Data Security Enabled |
| **Cloud** | AZURE |
| **Category** | SQL Server |
| **Description** | Ensures that Advanced Data Security is enabled for SQL Servers |
| **More Info** | Enabling Advanced Data Security on all SQL Servers ensures that SQL server data is encrypted and monitored for unusual activity, vulnerabilities, and threats. |
| **AZURE Link** | https://docs.microsoft.com/en-gb/azure/sql-database/sql-database-advanced-data-security |
| **Recommended Action** | Ensure that Advanced Data Security is enabled for all SQL Servers. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for SQL servers. </br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step2.png"/>
3. On the "SQL server" page, select the SQL server that needs to be examine. </br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step3.png"/>
4. On the selected "SQL server" page, scroll down the left navigation panel and select "Advanced data security" under the "Security" column.</br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step4.png"/>
5. On the "Advanced data security" page, if the "ADVANCED DATA SECURITY" is showing "OFF" then the selected "SQL server" does not ensured that SQL server data is encrypted and monitored for unusual activity, vulnerabilities, and threats. </br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "SQL servers" in the account.</br>
7. Navigate to "SQL servers", on the "SQL servers" page select the "SQL server", scroll down the left navigation panel and choose "Advanced data security" under the "Security."</br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step7.png"/>
8. On the "Advanced data security" page, click on the "ON" option next to the "ADVANCED DATA SECURITY". Select the "Subscription" and "Storage account" accordingly.</br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step8.png"/>
9. Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to ensure that Advanced Data Security is enabled for all SQL Servers.</br>
