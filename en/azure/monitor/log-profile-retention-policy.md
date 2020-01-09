[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Monitor / Log Profile Retention Policy

## Quick Info

| | |
|-|-|
| **Plugin Title** | Log Profile Retention Policy |
| **Cloud** | AZURE |
| **Category** | Monitor |
| **Description** | Ensures that Log Profiles have a long retention policy. |
| **More Info** | Log retention policies should be configured with sufficient retention to aid in investigation of prior security incidents and for compliance purposes. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitoring-overview-activity-logs#export-the-activity-log-with-a-log-profile |
| **Recommended Action** | Ensure that the Activity Log export to Event Hub is configured with a retention policy of at least 365 days. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Monitor. </br> <img src="/resources/azure/monitor/log-profile-retention-policy/step2.png"/>
3. Scroll down the left navigation panel and choose "Activity Log" option in the "Monitor" page.</br> <img src="/resources/azure/monitor/log-profile-retention-policy/step3.png"/>
4. On the "Monitor - Activity log" click on the "Export to Event Hub".</br> <img src="/resources/azure/monitor/log-profile-retention-policy/step4.png"/>
5. On the "Diagnostics settings" page select the diagnostic setting for which "Retention policy" needs to be verified and click on "Edit setting" option.</br> <img src="/resources/azure/monitor/log-profile-retention-policy/step5.png"/>
6. On the "Diagnostics settings" page select the "Storage account" option and check the "retention policy".If log "retention policy" is less than 90 days then it's not as per the Azure Recommendations.</br> <img src="/resources/azure/monitor/log-profile-retention-policy/step6.png"/>
7. Repeat steps number 2 - 6 to verify other Azure accounts for "Log Profile Retention Policy".</br>
8. Navigate to "Monitor" and click on the "Activity Log" under "Monitor page", click on the "Export to Event Hub" and select the "Diagnostic Setting" on which "Log Profile Retention Policy" needs to be set to at least 90 days.</br> <img src="/resources/azure/monitor/log-profile-retention-policy/step8.png"/>
9. Click on the "Edit Setting" option next to the "Diagnostic setting".</br> <img src="/resources/azure/monitor/log-profile-retention-policy/step9.png"/>
10. Click on the "Storage Account", select the "Region" and enter the "Retention(days)" to 90 and save the changes.</br> <img src="/resources/azure/monitor/log-profile-retention-policy/step10.png"/>
11. Repeat steps number 8 - 10 to ensure that the Activity Log export to Event Hub is configured with a retention policy of at least 90 days. </br>
