[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Monitor / Log Profile Archive Data

## Quick Info

| | |
|-|-|
| **Plugin Title** | Log Profile Archive Data |
| **Cloud** | AZURE |
| **Category** | Monitor |
| **Description** | Ensures the Log Profile is configured to export all activities from the control and management planes in all active locations |
| **More Info** | Exporting log activity for control plane activity allows for audited access to the Azure account with event data in the case of a security incident. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/azure-monitor/platform/archive-activity-log |
| **Recommended Action** | Ensure that all activity is logged to the Event Hub or storage account for archiving. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Log Analytics Workspaces". </br> <img src="/resources/azure/monitor/log-profile-archive-data/step2.png"/>
3. On the "Log Analytics workspaces" page select the resource and click on its Name to reach its configuration page.</br> <img src="/resources/azure/monitor/log-profile-archive-data/step3.png"/>
4. On the "Log Analytics workspaces - resource" page, scroll down the left navigation panel and choose "Activity Log".</br> <img src="/resources/azure/monitor/log-profile-archive-data/step4.png"/>
5. Click on the "Export Activity Logs" at the top of "Activity Log" page to ensures the "Log Profile" is configured.</br> <img src="/resources/azure/monitor/log-profile-archive-data/step5.png"/>
6. Under "Export Activity Logs" page, if no Diagnostic settings are defined, then the Log Profile is not configured to export all activities from control and management planes in all active locations. </br> <img src="/resources/azure/monitor/log-profile-archive-data/step6.png"/>
7. To ensure that all activity is logged to the Event Hub or storage account for archiving, on the "Export Activity Logs" page, click on the "Add diagnostic setting".</br> <img src="/resources/azure/monitor/log-profile-archive-data/step7.png"/>
8. Under the "Diagnostics Setting" page, enter the "Diagnostic setting name" and under "Destination details", click the checkbox for "Send to Log Analytics workspace", select a "Subscription" and an existing "Log Analytics workspace". </br> <img src="/resources/azure/monitor/log-profile-archive-data/step8.png"/>
9. Next, select the checkbox next to "Archive to a storage account" and select the "Subscription" and "Storage account" from the respective dropdowns.</br> <img src="/resources/azure/monitor/log-profile-archive-data/step9.png"/>
10. Choose the categories under "logs" accordingly.</br> <img src="/resources/azure/monitor/log-profile-archive-data/step10.png"/>
11. Click on the "Save" button at the top to make the necessary changes. </br> <img src="/resources/azure/monitor/log-profile-archive-data/step11.png"/>
12. Repeat steps number 5 - 11 to ensure that all activity is logged to the Event Hub or storage account for archiving.
