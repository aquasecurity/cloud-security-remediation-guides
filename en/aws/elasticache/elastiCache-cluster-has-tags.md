[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ElastiCache / ElastiCache Cluster Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | ElastiCache Cluster Has Tags |
| **Cloud** | AWS |
| **Category** | ElastiCache |
| **Description** | Ensure that ElastiCache clusters have tags |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonElastiCache/latest/red-ug/Tagging-Resources.html |
| **Recommended Action** | Modify ElastiCache cluster and add tags. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "ElastiCache" and Click on "ElastiCache". </br> <img src="/resources/aws/elasticache/elasticache-cluster-has-tags/step2.png"/>
3. On "ElastiCache Dashboard" page Click on Redis or MemCached Cluster according to your cluster type from left navigation panel. </br> <img src="/resources/aws/elasticache/elasticache-cluster-has-tags/step3.png"/>
4. On Redis/Memcached Clusters list page Click on the Cluster Name which needs to have tags. </br><img src="/resources/aws/elasticache/elasticache-cluster-has-tags/step4.png"/>
5. On Cluster details page choose "Tags" tab from navigation panel on the bottom of page. </br><img src="/resources/aws/elasticache/elasticache-cluster-has-tags/step7.png"/>
6. Under the "Tags" tab Click on "Manage Tags" button. </br><img src="/resources/aws/elasticache/elasticache-cluster-has-tags/step6.png"/>
7. On manage tags popup Click on "Add new tag" button. Enter the key-value for tag and Click "Apply" button to save the changes. </br><img src="/resources/aws/elasticache/elasticache-cluster-has-tags/step7.png"/>