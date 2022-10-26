[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ECS / ECS Clusters Have Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | ECS Cluster Has Tags |
| **Cloud** | AWS |
| **Category** | ECS |
| **Description** | Ensure ECS clusters have tags associated. |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage.|
| **AWS Link** | https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-using-tags.html |
| **Recommended Action** | Modify ECS Cluster and add tags. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for ECS. </br> <img src="/resources/aws/ecs/ecs-clusters-have-tags/step2.png"/>
3. In navigation pane select "Clusters".</br> <img src="/resources/aws/ecs/ecs-clusters-have-tags/step3.png"/>
4. On Clusters page click on the cluster name which needs to have tags.  </br> <img src="/resources/aws/ecs/ecs-clusters-have-tags/step4.png"/>
5. On Cluster Details page choose "Tags" tab from navigation panel. Under "Tags" tab click on "Edit" button. </br> <img src="/resources/aws/ecs/ecs-clusters-have-tags/step5.png"/>
6. On Tags pop up click enter key-value related to tag and Click on "Save".</br> <img src="/resources/aws/ecs/ecs-clusters-have-tags/step6.png"/>
