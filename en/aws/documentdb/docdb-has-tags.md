[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / DocumentDB / DocumentDB Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | DocumentDB Has Tags |
| **Cloud** | AWS |
| **Category** | DocumentDB |
| **Description** | Ensure that AWS DocumentDB clusters have tags associated. |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/documentdb/latest/developerguide/tagging.html |
| **Recommended Action** | Modify DocumentDB cluster and add tags. |

## Detailed Remediation Steps 
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "DocumentDB".</br> <img src="/resources/aws/documentdb/docdb-has-tags/step2.png"/>
3. On "DocumentDB Dashboard" page, Click on "Clusters" from left navigation panel.</br> <img src="/resources/aws/documentdb/docdb-has-tags/step3.png"/>
4. On Documentdb clusters list page, Click on the cluster name which needs to have tags.</br> <img src="/resources/aws/documentdb/docdb-has-tags/step4.png"/>
5. On Cluster details page scroll down and click on the "Events & tags" tab from the bottom panel.</br> <img src="/resources/aws/documentdb/docdb-has-tags/step5.png"/>
6. Under "Events & tags" tab scroll down to "Tags" section. Click on "Manage Tags" button to manage new tags.</br> <img src="/resources/aws/documentdb/docdb-has-tags/step6.png"/>
7. On "Manage Tags" page click on "Add new tags" button and enter key-value for the tag and Click on "Save" button.</br> <img src="/resources/aws/documentdb/docdb-has-tags/step7.png"/> 
