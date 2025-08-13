[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Monitor / Log Analytics Workspace Public Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Log Analytics Public Workspace |
| **Cloud** | AZURE |
| **Category** | Monitor |
| **Description** | Ensures Log Analytics Workspace is not publicly accessible |
| **More Info** | Securing Log Analytics workspaces through private links, and disallowing public access, enhances data protection, access control, and overall security by restricting entry to authorized networks and minimizing potential external threats. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/azure-monitor/logs/private-link-configure#configure-access-to-your-resources |
| **Recommended Action** | Configure Log Analytics workspaces with private links and deny access from public networks. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Log Analytics workspaces". </br> 
3. On the "Log Analytics Workspaces" page select the resource and click on its Name to reach its configuration page.</br>
<img src="/resources/azure/monitor/log-analytics-workspace-public/step1.png"/>  
4. On the "Log Analytics Workspaces - resource" page, scroll down the left navigation panel and choose "Network Isolation".</br> <img src="/resources/azure/monitor/log-analytics-workspace-public/step2.png"/> 
5. Under "Public access" tab, you will see "Ingestion access" and "Query access" sections. Click on the "Manage" button to configure public network access.</br>
6. In the "Public network access" pop-up window that appears, under "Ingestion access", select "Secured by perimeter" to disable public ingestion access.</br>
7. Under "Query access", select "Secured by perimeter" to disable public query access.</br> <img src="/resources/azure/monitor/log-analytics-workspace-public/step3.png"/>
8. Click on the "Save" button to apply the changes.</br>


