
[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Networks / Route Table Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | Route Table Has Tags |
| **Cloud** | AZURE |
| **Category** | Virtual Networks |
| **Description** | Ensures that Microsoft Azure Route Table has tags associated. |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/tag-resources |
| **Recommended Action** | Modify route table and add tags |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. In search bar at the top search for route tables and select "Route Tables". </br> <img src="/resources/azure/virtualnetworks/routeTable-has-tags/step2.png"/>
3. Select a route table by clicking on the "Name" link to load the configuration pane.</br> <img src="/resources/azure/virtualnetworks/routeTable-has-tags/step3.png"/>
4. On the configuration pane, choose "Tags" from the left navigation panel. </br>  <img src="/resources/azure/virtualnetworks/routeTable-has-tags/step4.png"/>
5. On "Tags" page enter the name/value of the tag you want to add and click "Apply" on the bottom of the page" </br> <img src="/resources/azure/virtualnetworks/routeTable-has-tags/step5.png"/>
