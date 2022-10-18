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

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "SQL servers". </br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step2.png"/>
3. On the "SQL server" page, select the SQL server that needs to be examined. </br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step3.png"/>
4. On the selected "SQL server" page, scroll down the left navigation panel and select "Microsoft defender for cloud" under "Security".</br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step4.png"/>
5. On the "Microsoft Defender for Cloud" page, if the "Microsoft Defender for SQL" is showing "Disabled" then the selected "SQL server" does not ensure that the server data is encrypted and monitored for unusual activity, vulnerabilities and threats. </br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step5.png"/>
6. To ensure that Advanced Data Security is enabled for the selected server, on the "Microsoft Defender for Cloud" page, click on "Configure" infront of "Microsoft Defender for SQL" to reach its configuration page.</br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step6.png"/>
7. On the "Server settings" page, toggle the switch to "ON" under "MICROSOFT DEFENDER FOR SQL". Select the "Subscription" and "Storage account" accordingly.</br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step7.png"/>
8. Click on the "Save" button at the top to make the necessary changes.</br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step8.png"/>
9. Repeat steps number 3 - 8 to ensure that Advanced Data Security is enabled for all SQL Servers.</br>
