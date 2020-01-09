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

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Log Analytics Workspace. </br> <img src="/resources/azure/monitor/log-profile-archive-data/step2.png"/>
3. On the "Log Analytics workspaces" page select the resource accordingly.</br> <img src="/resources/azure/monitor/log-profile-archive-data/step3.png"/>
4. On the "Log Analytics workspaces - resource" page, scroll down the left navigation panel and choose "Activity Log".</br> <img src="/resources/azure/monitor/log-profile-archive-data/step4.png"/>
5. Click on the "Export to Event Hub" at the top of "Activity Log" page to ensures the "Log Profile" is configured.</br> <img src="/resources/azure/monitor/log-profile-archive-data/step5.png"/>
6. Under "Export to Event Hub" page, if there are no Diagnostic settings are defined, then the Log Profile is not configured to export all activities from the control and management planes in all active locations. </br> <img src="/resources/azure/monitor/log-profile-archive-data/step6.png"/>
7. Repeat steps number 2 - 6 to verify "Log Profiles" of another Azure account.</br>
8. Navigate to "Log Analytics Workspace" and select the resource, and choose "Activity Log" from the left navigation panel and click on the "Export to Event Hub".</br> <img src="/resources/azure/monitor/log-profile-archive-data/step8.png"/>
9. On the "Export to Event Hub" page, click on the "Add diagnostic setting".</br> <img src="/resources/azure/monitor/log-profile-archive-data/step9.png"/>
10. Under the "Diagnostics Setting" page, enter the Name, select the checkbox next to "Archive to a storage account" option and click on the "Configure" under "Storage account".</br> <img src="/resources/azure/monitor/log-profile-archive-data/step10.png"/>
11. On the "Storage account" select the "Subscription" and "Storage account" from the respective dropdown and click on "OK" at the bottom of the page.</br> <img src="/resources/azure/monitor/log-profile-archive-data/step11.png"/>
12. On the "Diagnostics Settings" page enter the Name, click the checkbox for "Send to Log Analytics", select an existing Log Analytics workspace, or create a workspace and select the log type accordingly.</br> <img src="/resources/azure/monitor/log-profile-archive-data/step12.png"/>
13. Click on the "Save" button at the top to make the necessary changes. </br> <img src="/resources/azure/monitor/log-profile-archive-data/step13.png"/>
14. Repeat steps number 8 - 13 to ensure that all activity is logged to the Event Hub or storage account for archiving.
