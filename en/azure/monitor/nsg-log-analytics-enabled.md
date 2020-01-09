[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Monitor / NSG Log Analytics Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | NSG Log Analytics Enabled |
| **Cloud** | AZURE |
| **Category** | Monitor |
| **Description** | Ensures Network Security Group logs are sent to the Log Analytics workspace |
| **More Info** | Enabling Log Analytics for Network Security Groups ensures that logs are shipped to a central repository that can be queried and audited. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/azure-monitor/platform/collect-activity-logs |
| **Recommended Action** | Enable sending of logs to Log Analytics for each Network Security Group resource in the Azure Monitor. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Network Security Group. </br> <img src="/resources/azure/monitor/nsg-log-analytics-enabled/step2.png"/>
3. Select the "Network Security Group" which needs to be verified.</br> <img src="/resources/azure/monitor/nsg-log-analytics-enabled/step3.png"/>
4. On the "Network security groups" page, scroll down the left navigation panel and choose "Diagnostics Settings" under "Monitoring".</br> <img src="/resources/azure/monitor/nsg-log-analytics-enabled/step4.png"/>
5. On the "Network security groups - Diagnostic Setting" page if "No diagnostic settings defined" is showing then the select "Network Security Group" then logs are not sent to the Log Analytics workspace.</br> <img src="/resources/azure/monitor/nsg-log-analytics-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Network Security Groups".</br>
7. Navigate to "Network Security Group", select the "Network Security Group" and choose "Diagnostics Settings" under "Monitoring".</br> <img src="/resources/azure/monitor/nsg-log-analytics-enabled/step7.png"/>
8. On the "Diagnostic settings" page click on the "Add diagnostic setting" option.</br> <img src="/resources/azure/monitor/nsg-log-analytics-enabled/step8.png"/>
9. On the "Diagnostics Settings" page enter the Name, click the checkbox for "Send to Log Analytics", select an existing Log Analytics workspace, or create a workspace and to enable "log" and select the checkboxes against "NetworkSecurityGroupEvent" and "NetworkSecurityGroupRuleCounter". Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/monitor/nsg-log-analytics-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to enable sending of logs to Log Analytics for each Network Security Group resource in the Azure Monitor.</br>
