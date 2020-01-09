[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Monitor / Key Vault Log Analytics Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Key Vault Log Analytics Enabled |
| **Cloud** | AZURE |
| **Category** | Monitor |
| **Description** | Ensures Key Vault Log Analytics logs are being properly delivered to Azure Monitor |
| **More Info** | Enabling Send to Log Analytics ensures that all Key Vault logs are being properly monitored and managed. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/azure-monitor/platform/collect-activity-logs |
| **Recommended Action** | Send all diagnostic logs for Key Vault from the Azure Monitor service to Log Analytics. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Monitor. </br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step2.png"/>
3. On the "Monitor - Overview" page scroll down the left navigation panel and click on "Diagnostics" under Settings.</br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step3.png"/>
4. On the "Monitor - Diagnostics settings" page select the resource you want to verify for "Key Vault Log Analystics."</br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step4.png"/>
5. Check the "Diagnostics Status" and if it's set to "Disabled" then the  "Key Vault Log Analytics" logs are not being properly delivered to Azure Monitor.</br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other resources in the account.</br>
7. Navigate to "Monitor" and click on the "Diagnostics" under "Settings" and select the resource on which "Key Vault Log Anaytics" needs to be enabled.</br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step7.png"/>
8. On the "Diagnostics Settings" page click on the "Add diagnostic setting" option.</br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step8.png"/>
9. On the "Diagnostics Settings" page enter the Name, click the checkbox for "Send to Log Analytics", select an existing Log Analytics workspace, or create a workspace and to enable "Metric" click the checkbox under "Metric". Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to send all diagnostic logs for Key Vault from the Azure Monitor service to Log Analytics.</br>
