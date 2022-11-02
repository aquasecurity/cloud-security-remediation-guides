[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / VPC Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | VPC Has Tags |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensure VPC have tags associated. |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://aws.amazon.com/about-aws/whats-new/2020/07/amazon-vpc-resources-support-tag-on-create/ |
| **Recommended Action** | Modify VPC and add new tags. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for VPC. </br> <img src="/resources/aws/ec2/vpc-has-tags/step2.png"/>
3. Scroll down the left navigation panel and choose "Your VPC" under "Virtual Private Cloud". </br> <img src="/resources/aws/ec2/vpc-has-tags/step3.png"/>
4. On "Your VPC" page Click on the vpc which needs to have tags.</br>  <img src="/resources/aws/ec2/vpc-has-tags/step4.png"/>
5. On VPC details page choose "Tags" tab from the navigation panel on bottom of the page. </br> <img src="/resources/aws/ec2/vpc-has-tags/step5.png"/>
6. Under the "Tags" tab click on "Manage Tags" button. </br>  <img src="/resources/aws/ec2/vpc-has-tags/step6.png"/>
7. On "Manage Tags" page Click on "Add new tag" button, and enter key-value pair for the tag, then Click on "Save".</br> <img src="/resources/aws/ec2/vpc-has-tags/step7.png"/>
