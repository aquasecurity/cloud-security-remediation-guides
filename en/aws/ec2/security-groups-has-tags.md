[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Security Groups Have Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | Security Group has Tags |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensure that AWS Security Groups have tags associated. |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://aws.amazon.com/about-aws/whats-new/2021/07/amazon-ec2-adds-resource-identifiers-tags-vpc-security-groups-rules/ |
| **Recommended Action** | Update Security Group and add Tags |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "Security Groups". </br> <img src="/resources/aws/ec2/security-groups-has-tags/step2.png"/>
3. On Security Groups page Click on the security group which needs to have tags. </br>  <img src="/resources/aws/ec2/security-groups-has-tags/step3.png"/>
4. On the security group details page Choose "Tags" from the navigation panel in the middle of the page.</br> <img src="/resources/aws/ec2/security-groups-has-tags/step4.png"/>
5. Under "Tags" tab Click on "Manage Tags" button.</br> <img src="/resources/aws/ec2/security-groups-has-tags/step5.png"/>
6. On "Manage Tags" page click on "Add new tag" then enter the key and value pair for the tag and Click on "Save changes" button.</br><img src="/resources/aws/ec2/security-groups-has-tags/step6.png"/>