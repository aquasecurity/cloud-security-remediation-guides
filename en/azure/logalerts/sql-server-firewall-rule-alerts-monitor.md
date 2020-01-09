[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Log Alerts / SQL Server Firewall Rule Alerts Monitor

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQL Server Firewall Rule Alerts Monitor |
| **Cloud** | AZURE |
| **Category** | Log Alerts |
| **Description** | Ensures Activity Log Alerts for the create or update and delete SQL Server Firewall Rules events are enabled |
| **More Info** | Monitoring for create or update and delete SQL Server Firewall Rules events gives insight into event changes and may reduce the time it takes to detect suspicious activity. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/sql-database/sql-database-firewall-configure |
| **Recommended Action** | Add a new log alert to the Alerts service that monitors for SQL Server Firewall Rules create or update and delete events. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Alerts. </br> <img src="/resources/azure/logalerts/sql-server-firewall-rule-alerts-monitor/step2.png"/>
3. On the "Alerts" page, click on the "Manage alert rules" at the top panel.</br> <img src="/resources/azure/logalerts/sql-server-firewall-rule-alerts-monitor/step3.png"/>
4. On the "Rules" page, scroll down the page and check the "Target Resource Type" and check if there is any rules for "SQL Server Firewall Alerts". If there is no "Alerts" configured then "Activity Log Alerts" for the create or update and delete "SQL Server Firewall Rules" events are not enabled.</br> <img src="/resources/azure/logalerts/sql-server-firewall-rule-alerts-monitor/step4.png"/>
5. Repeat steps number 2 - 4 to check other Azure accounts.</br>
6. Navigate to the "Alerts" and click on the "New alert rule" at the top.</br> <img src="/resources/azure/logalerts/sql-server-firewall-rule-alerts-monitor/step6.png"/>
7. On the "Create rule" page, click on the "Select" option under the "Resources" and search for "SQL Server" from the "Filter by resource type" and select the "Resource" accordingly.</br> <img src="/resources/azure/logalerts/sql-server-firewall-rule-alerts-monitor/step7.png"/>
8. On the "Create rule" page, click on the "Add" option under the "Condition" and select "All Administrative operations" from the options and click on the "Done" option at the bottom of the tab.</br> <img src="/resources/azure/logalerts/sql-server-firewall-rule-alerts-monitor/step8.png"/>
9. Under the "Actions", select the "Action group" or "Create action group" accordingly.</br> <img src="/resources/azure/logalerts/sql-server-firewall-rule-alerts-monitor/step9.png"/>
10. Enter the "Alert rule name" and "Description" under the "Alert Details" and click on the "Yes" button under the "Enable rule upon creation" to quickly enable the "SQL Server Firewall Rule Alerts". Click on the "Create alert rule" button at the bottom to create a rule.</br> <img src="/resources/azure/logalerts/sql-server-firewall-rule-alerts-monitor/step10.png"/>
11. Repeat steps number 6 - 10 to add a new log alert to the Alerts service that monitors for SQL Server Firewall Rules create or update and delete events.</br>
