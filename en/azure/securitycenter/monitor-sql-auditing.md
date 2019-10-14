[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Security Center / Monitor SQL Auditing

## Quick Info

| | |
|-|-|
| **Plugin Title** | Monitor SQL Auditing |
| **Cloud** | AZURE |
| **Category** | Security Center |
| **Description** | Ensures that Monitor SQL Auditing is enabled in Security Center |
| **More Info** | When this setting is enabled, Security Center will monitor SQL databases. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-policy-definitions |
| **Recommended Action** | Ensure SQL auditing monitoring is configured for SQL databases from the Azure Security Center. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Security Center. </br> <img src="/resources/azure/securitycenter/monitor-sql-auditing/step2.png"/>
3. Scroll down the "Security Center" navigation panel and select the "Security policy" option under "POLICY & COMPLIANCE."</br> <img src="/resources/azure/securitycenter/monitor-sql-auditing/step3.png"/>
4. On the "Policy Management" page under "Name" column select the "Subscription Name" that needs to be verified.</br> <img src="/resources/azure/securitycenter/monitor-sql-auditing/step4.png"/>
5. On the "Security Policy" page scroll down the "Data" section and check the "Monitor unaudited SQL servers in Azure Security Center". If it's set to "Disabled" then "Monitor SQL Auditing" is not enabled on the selected "Subscription."</br> <img src="/resources/azure/securitycenter/monitor-sql-auditing/step5.png"/>
6. Repeat steps number 2 - 5 to check other "Subscriptions" under the "Security Center."</br>
7. Navigate to the "Security Center", select the "Security policy" and under "Policy Management" seelct the "Subscription" that needs to enable the "SQL Auditing."</br> <img src="/resources/azure/securitycenter/monitor-sql-auditing/step7.png"/>
8. Select the "Subscription" link under the "Security policy" at the top to get into the configuration settings. </br> <img src="/resources/azure/securitycenter/monitor-sql-auditing/step8.png"/>
9. Scroll down the page and under "Parameter" choose the "Monitor unaudited SQL servers in Azure Security Center" and select the "AuditIfNotExists" option from the dropdown menu and click on the "Save" button at the bottom to make the necessary changes.</br> <img src="/resources/azure/securitycenter/monitor-sql-auditing/step9.png"/>
10. Repeat steps number 7 - 9 to ensures "Monitor SQL Auditing" is enabled in Security Center.</br>
