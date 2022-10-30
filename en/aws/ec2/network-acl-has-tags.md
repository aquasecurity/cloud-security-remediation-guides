[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Network ACL Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | Network ACL Has Tags |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensure that Network ACLs have tags |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html |
| **Recommended Action** | Update Network ACL and Add Tags |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for VPC. </br> <img src="/resources/aws/ec2/network-acl-has-tags/step2.png"/>
3. Scroll down the left navigation panel and choose "Network ACL" under "Security". </br> <img src="/resources/aws/ec2/network-acl-has-tags/step3.png"/>
4. Select the "Network ACL" that needs to have tags and choose the "Tags" tab from navigation panel on the bottom of page. </br> <img src="/resources/aws/ec2/network-acl-has-tags/step5.png"/>
5. Under Tags click on "Manage Tags" button . </br>
6. On Manage Tags page Click on "Add new Tags" button. Enter the key value for tags and click "Save".</br> <img src="/resources/aws/ec2/network-acl-has-tags/step7.png"/>