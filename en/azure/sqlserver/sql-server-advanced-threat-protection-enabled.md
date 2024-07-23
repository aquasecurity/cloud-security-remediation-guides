[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Server / SQL Server Advanced Threat Protection Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQL Server Advanced Threat Protection Enabled |
| **Cloud** | AZURE |
| **Category** | SQL Server |
| **Description** | Ensures that Advanced Threat Protection is enabled on SQL Servers. |
| **More Info** | Azure Defender for SQL is a unified package for advanced SQL security capabilities. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/azure-sql/database/azure-defender-for-sql |
| **Recommended Action** | Ensure that ThreatDetectionState is set to Enabled. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "SQL servers". </br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step2.png"/>
3. On the "SQL server" page, select the SQL server that needs to be examined. </br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step3.png"/>
4. On the selected "SQL server" page, scroll down the left navigation panel and select "Microsoft defender for cloud" under "Security".</br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step4.png"/>
5. On the "Microsoft Defender for Cloud" page, if the "Microsoft Defender for SQL" is  "Disabled" then the selected "SQL server" does not ensure that the server data is encrypted and monitored for unusual activity, vulnerabilities and threats. </br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step5.png"/>
6. To ensure that Advanced Threat Protection is enabled for the selected server, on the "Microsoft Defender for Cloud" page, click on "Enabled" button to enable the Microsoft Defender for SQL.</br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step6.png"/>
7. Once  the Microsoft Defender is enable , you can see the vulnerabilities and threats.</br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step7.png"/>
8. On the "Microsoft Defender for Cloud" page, click on "Configure" next to Enabled at the subscription-level.</br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step8.png"/>
9. Here we can see by enabling Microsoft Defender for SQL , Vulnerability Assessment and Advanced Threat Protection are also enabled.</br> <img src="/resources/azure/sqlserver/advanced-data-security-enabled/step9.png"/>
10. Repeat steps number 3 - 6 to ensure that Advanced Threat Protection is enabled for all SQL Servers.</br>
