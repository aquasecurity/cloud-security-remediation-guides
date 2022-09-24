[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Instance Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance Has Tags |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensure EFS File systems have tags |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Using_Tags.html |
| **Recommended Action** | Add tags for ec2 instance |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/ec2-has-tags/step2.png"/>
3. Scroll down the left navigation panel and choose "Instances". </br>  <img src="/resources/aws/ec2/ec2-has-tags/step3.png"/>
4. Select the "EC2 Instance" for which you want to add tags and click on the "Tags" tab in navigation panel below. </br> <img src="/resources/aws/ec2/ec2-has-tags/step4.png"/>
5. On the "Description" tab Click on "Manage Tags" button </br> <img src="/resources/aws/ec2/ec2-has-tags/step5.png"/>
6. On "Manage Tags" page click on "Add Tag" button enter key and value for your tag and click save.</br> <img src="/resources/aws/efs/ec2-has-tags/step6.png"/>


