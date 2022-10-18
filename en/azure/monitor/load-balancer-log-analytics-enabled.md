[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Monitor / Load Balancer Log Analytics Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Load Balancer Log Analytics Enabled |
| **Cloud** | AZURE |
| **Category** | Monitor |
| **Description** | Ensures Load Balancers Log Analytics logs are being properly delivered to Azure Monitor |
| **More Info** | Enabling Send to Log Analytics ensures that all Load Balancer logs are being properly monitored and managed. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/azure-monitor/platform/collect-activity-logs |
| **Recommended Action** | Send all diagnostic logs for Load Balancers from the Azure Monitor service to Log Analytics. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Load balancers". </br> <img src="/resources/azure/monitor/load-balancer-log-analytics-enabled/step2.png"/>
3. Select the "Load balancer" which needs to be verified and click on its Name to reach its configuration settings page.</br> <img src="/resources/azure/monitor/load-balancer-log-analytics-enabled/step3.png"/>
4. On the "Load balancer" page, scroll down the left navigation panel and choose "Diagnostics Settings" under "Monitoring".</br> <img src="/resources/azure/monitor/load-balancer-log-analytics-enabled/step4.png"/>
5. On the "Load balancer - Diagnostic Settings" page if "No diagnostic settings defined" is showing then the selected "Load balancer" logs are not sent to the Log Analytics workspace.</br> <img src="/resources/azure/monitor/load-balancer-log-analytics-enabled/step5.png"/>
6. To enable "Load Balancer Log Analytics" click on the "Add diagnostic setting" option.</br> <img src="/resources/azure/monitor/load-balancer-log-analytics-enabled/step6.png"/>
7. On the "Diagnostics Settings" page, enter the Name, click the checkbox for "Send to Log Analytics workspace", select an existing Log Analytics workspace, or create a workspace to enable logs. Under "Metrics" select the checkbox for "AllMetrics".</br> <img src="/resources/azure/monitor/load-balancer-log-analytics-enabled/step7.png"/>
8. Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/monitor/load-balancer-log-analytics-enabled/step8.png"/>
9. Repeat step number 3 - 8 to send all diagnostic logs for Load Balancers from the Azure Monitor service to Log Analytics.
