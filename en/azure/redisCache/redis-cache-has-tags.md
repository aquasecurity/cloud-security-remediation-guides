
[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Redis Cache / Redis Cache Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | Redis Cache Has Tags |
| **Cloud** | AZURE |
| **Category** | Redis Cache |
| **Description** | Ensures that Azure Cache for Redis have tags associated. |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/tag-resources |
| **Recommended Action** | Modify Azure Cache for Redis and add tags. |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. In search bar at the top, search for Redis Cache and select "Azure Cache for Redis" from search results. </br> <img src="/resources/azure/redisCache/redis-cache-has-tags/step2.png"/>
3. Select a redis cache by clicking on the "Name" link to load the configuration pane.</br> <img src="/resources/azure/redisCache/redis-cache-has-tags/step3.png"/>
4. On the configuration pane, choose "Tags" from the left navigation panel. </br>  <img src="/resources/azure/redisCache/redis-cache-has-tags/step4.png"/>
5. On "Tags" page enter the name/value of the tag you want to add and click "Apply" on the bottom of the page". </br> <img src="/resources/azure/redisCache/redis-cache-has-tags/step5.png"/>
