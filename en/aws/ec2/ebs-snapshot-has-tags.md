[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / EBS Snapshot Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | EBS Snapshot Has Tags |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensure that EBS snapshots have tags |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://aws.amazon.com/blogs/compute/tag-amazon-ebs-snapshots-on-creation-and-implement-stronger-security-policies/ |
| **Recommended Action** | Modify EBS snapshots and add tags. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/ebs-snapshot-has-tags/step2.png"/>
3. Scroll down the left navigation panel and choose "Snapshots". </br>  <img src="/resources/aws/ec2/ebs-snapshot-has-tags/step3.png"/>
4. Select the "Snapshot" that needs to have tags and click on its name from the "Name" column.</br> <img src="/resources/aws/ec2/ebs-snapshot-has-tags/step4.png"/>
5. Scroll down the page and under "Tags" tab Click on "Manage Tags" button.</br> <img src="/resources/aws/ec2/ebs-snapshot-has-tags/step5.png"/>
6. On "Manage tags" page Click on "Add Tag" button and enter the key-value for tag and Click "Save" button.</br><img src="/resources/aws/ec2/ebs-snapshot-has-tags/step6.png"/>
