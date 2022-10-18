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

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Monitor". </br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step2.png"/>
3. On the "Monitor - Overview" page scroll down the left navigation panel and click on "Diagnostic settings" under Settings.</br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step3.png"/>
4. On the "Monitor - Diagnostics settings" page select the resource you want to verify for "Key Vault Log Analystics."</br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step4.png"/>
5. Check the "Diagnostics Status" of the chosen resource and if it's set to "Disabled" then the  "Key Vault Log Analytics" logs are not being properly delivered to Azure Monitor.</br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step5.png"/>
6. To enable "Key Vault Log Anaytics" on the selected resource click on the resource name to reach its configuration settings page </br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step6.png"/>
7. Under the "Diagnostics Settings" click on the "Add diagnostic setting" option.</br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step7.png"/>
8. On the next page, enter the "Diagnostic setting name". Under "Logs" checkmark "alllogs". Under "Destination details" click the checkbox for "Send to Log Analytics workspace", select an existing "Subscription" & "Log Analytics workspace", or create a workspace.</br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step8.png"/>
9. Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step9.png"/>
10. "Key Vault Log Anaytics" is now enabled for the selected resource.</br> <img src="/resources/azure/monitor/key-vault-log-analytics-enabled/step10.png"/>
11. Repeat steps number 6 - 9 to send all diagnostic logs for Key Vault from the Azure Monitor service to Log Analytics.</br>
