[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / DocumentDB / DocumentDB Cluster Deletion Protection

## Quick Info

| | |
|-|-|
| **Plugin Title** | DocumentDB Cluster Deletion Protection |
| **Cloud** | AWS |
| **Category** | DocumentDB |
| **Description** | Ensure that Amazon DocumentDB clusters have deletion protection feature enabled. |
| **More Info** | Enabling deletion protection feature for Amazon DocumentDB clusters acts as a safety net, preventing accidental database deletions or deletion by an unauthorized user. It ensures that the data stays secure and accessible at all times. |
| **AWS Link** | https://docs.aws.amazon.com/documentdb/latest/developerguide/db-cluster-delete.html |
| **Recommended Action** | Modify DocumentDB cluster and enable deletion protection. |

## Detailed Remediation Steps 
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "DocumentDB".</br> <img src="/resources/aws/documentdb/docdb-deletion-protection/step2.png"/>
3. On "DocumentDB Dashboard" page, Click on "Clusters" from left navigation panel.</br> <img src="/resources/aws/documentdb/docdb-deletion-protection/step3.png"/>
4. On DocumentDB clusters list page, Click on the cluster name on which you want to enable deletion protection feature.</br> <img src="/resources/aws/documentdb/docdb-deletion-protection/step4.png"/>
5. On Cluster details page scroll down and go to the "Configuration" tab from the bottom panel and click on "Modify" button.</br> <img src="/resources/aws/documentdb/docdb-deletion-protection/step5.png"/>
6. Scroll to bottom of "Modify Cluster" page and under "Deletion protection" section, check the "Enable deletion protection" checkbox and click "Continue" button.</br> <img src="/resources/aws/documentdb/docdb-deletion-protection/step6.png"/>
7. On "Scheduling of modifications" section check "Apply immediately" checkbox and click on "Modify Cluster" button.</br> <img src="/resources/aws/documentdb/docdb-deletion-protection/step7.png"/> 
