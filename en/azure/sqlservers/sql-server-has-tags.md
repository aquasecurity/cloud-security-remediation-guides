
[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Servers / SQL Server Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQL Server Has Tags |
| **Cloud** | AZURE |
| **Category** | SQL Servers |
| **Description** | Ensures that Azure SQL Server have tags associated |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/tag-resources |
| **Recommended Action** | Modify SQL Server and tags. |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for SQL servers. </br> <img src="/resources/azure/sqlservers/sql-server-has-tags/step2.png"/>
3. On the "SQL server" page, select the SQL server that needs to be examine.</br><img src="/resources/azure/sqlservers/sql-server-has-tags/step3.png"/>
4. On the selected "SQL server" page, select "Tags" from the left navigation panel."</br> <img src="/resources/azure/sqlservers/sql-server-has-tags/step4.png"/>
5. On "Tags" page enter the name/value of the tag you want to add and click "Apply" on the bottom of the page" </br> <img src="/resources/azure/sqlservers/sql-server-has-tags/step5.png"/>
