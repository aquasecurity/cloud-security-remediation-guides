[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Public AMI

## Quick Info

| | |
|-|-|
| **Plugin Title** | AMI have Tags |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensure that AMIs have tags |
| **More Info** |Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://aws.amazon.com/about-aws/whats-new/2020/12/amazon-machine-images-support-tag-on-create-tag-based-access-control/ |
| **Recommended Action** | Modify AMI and add tags. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/ami-has-tags/step2.png"/>
3. Scroll down the left navigation panel and choose "AMIs" under "Images".</br> <img src="/resources/aws/ec2/ami-has-tags/step3.png"/>
4. Select the "AMI" that needs to have tags. </br> <img src="/resources/aws/ec2/ami-has-tags/step4.png"/>
5. Scroll down the page and select the "Tags" tab from the dashboard bottom panel and Click on "Manage Tags".</br> <img src="/resources/aws/ec2/ami-has-tags/step5.png"/>
6. On Manage Tags page click on "Add Tags" and enter the key-value for the tag and Click "Save".</br><img src="/resources/aws/ec2/ami-has-tags/step6.png"/>
