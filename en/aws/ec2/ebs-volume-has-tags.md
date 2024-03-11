[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / EBS Volume has tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | EBS Volume has tags |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensure that EBS Volumes have tags associated |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://aws.amazon.com/blogs/aws/new-tag-ec2-instances-ebs-volumes-on-creation/ |
| **Recommended Action** | Modify EBS volumes and add tags |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/ebs-volume-has-tags/step2.png"/>
3. Scroll down the left navigation panel and choose "Volumes". </br>  <img src="/resources/aws/ec2/ebs-volume-has-tags/step3.png"/>
4. Select the "Volume" that needs to have tags and click on its name from the "Name" column.</br> <img src="/resources/aws/ec2/ebs-volume-has-tags/step4.png"/>
5. Scroll down the page and under "Tags" tab Click on "Manage Tags" button</br> <img src="/resources/aws/ec2/ebs-volume-has-tags/step5.png"/>
6. On "Manage tags" page Click on "Add Tag" button and enter the key-value for tag and Click "Save" button.</br><img src="/resources/aws/ec2/ebs-volume-has-tags/step6.png"/>
