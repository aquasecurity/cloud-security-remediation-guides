[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Log Alerts / Security Solution Logging

## Quick Info

| | |
|-|-|
| **Plugin Title** | Security Solution Logging |
| **Cloud** | AZURE |
| **Category** | Log Alerts |
| **Description** | Ensures Activity Log Alerts for the create or update and delete Security Solution events are enabled |
| **More Info** | Monitoring for create or update and delete Security Solution events gives insight into event changes and may reduce the time it takes to detect suspicious activity. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security/azure-log-audit |
| **Recommended Action** | Add a new log alert to the Alerts service that monitors for Security Solution create or update and delete events. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Alerts. </br> <img src="/resources/azure/logalerts/security-solution-logging/step2.png"/>
3. On the "Alerts" page, click on the "Manage alert rules" at the top panel.</br> <img src="/resources/azure/logalerts/security-solution-logging/step3.png"/>
4. On the "Rules" page, scroll down the page and check the "Target Resource Type" and check if there is any rules for "Security Solutions (securitySolutions)". If there is no "Alerts" configured then "Security Solutions (securitySolutions)" for the create or update and delete "Security Solutions (securitySolutions)" events are not enabled.</br> <img src="/resources/azure/logalerts/security-solution-logging/step4.png"/>
5. Repeat steps number 2 - 4 to check other Azure accounts.</br>
6. Navigate to the "Alerts" and click on the "New alert rule" at the top.</br> <img src="/resources/azure/logalerts/security-solution-logging/step6.png"/>
7. On the "Create rule" page, click on the "Select" option under the "Resources" and search for "Security Solutions (securitySolutions)" from the "Filter by resource type" and select the "Resource" accordingly.</br> <img src="/resources/azure/logalerts/security-solution-logging/step7.png"/>
8. On the "Create rule" page, click on the "Add" option under the "Condition" and select "All Security operations" from the options and click on the "Done" option at the bottom of the tab.</br> <img src="/resources/azure/logalerts/security-solution-logging/step8.png"/>
9. Under the "Actions", select the "Action group" or "Create action group" accordingly.</br> <img src="/resources/azure/logalerts/security-solution-logging/step9.png"/>
10. Enter the "Alert rule name" and "Description" under the "Alert Details" and click on the "Yes" button under the "Enable rule upon creation" to quickly enable the "Security Solutions (securitySolutions)". Click on the "Create alert rule" button at the bottom to create a rule.</br> <img src="/resources/azure/logalerts/security-solution-logging/step10.png"/>
11. Repeat steps number 6 - 10 to add  a new log alert to the Alerts service that monitors for Security Solution create or update and delete events.</br>
