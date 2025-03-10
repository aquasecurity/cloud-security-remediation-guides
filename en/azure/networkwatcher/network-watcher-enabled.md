[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Network Watcher / Network Watcher Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Network Watcher Enabled |
| **Cloud** | AZURE |
| **Category** | Network Watcher |
| **Description** | Ensures Network Watcher is enabled in all locations |
| **More Info** | Network Watcher helps locate, diagnose, and gain insights into Azure networks. Enabling Network Watcher in all locations ensures that no resources are being used in locations that are not authorized. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/network-watcher/network-watcher-monitoring-overview |
| **Recommended Action** | Enable the Network Watcher service in all locations. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Network Watcher. </br> <img src="/resources/azure/networksecuritygroups/network-watcher-enabled/step2.png"/>
3. On the "Network Watcher" page, click on the Overview tab and check the status of the "Network Watcher."</br> <img src="/resources/azure/networksecuritygroups/network-watcher-enabled/step3.png"/>
4. On the "Overveiw" tab if you do not see any Network watcher listed then you do not have any Network Watcher enabled. </br> <img src="/resources/azure/networksecuritygroups/network-watcher-enabled/step4.png"/>
5. Repeat step number 2 - 4 to check the status of Network Watcher in other Azure accounts.</br> 
6. Navigate to "Network Watcher" and click on the Overview page. Click on the "Add" button at the top to create a Network watcher. </br> <img src="/resources/azure/networksecuritygroups/network-watcher-enabled/step6.png"/>
7. On the "Add network watcher" pane that opens on the right, choose the "Subscription" and then click on  "Select All" to select all locations under "Region".</br> <img src="/resources/azure/networksecuritygroups/network-watcher-enabled/step7.png"/>
8. Click "Add" button at the bottom of the screen to create your Network watcher.</br> <img src="/resources/azure/networksecuritygroups/network-watcher-enabled/step8.png"/>
9. Now we have a Network Watcher service Enabled for all locations.</br> <img src="/resources/azure/networksecuritygroups/network-watcher-enabled/step9.png"/>

