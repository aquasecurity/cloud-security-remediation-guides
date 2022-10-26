[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ELB / ELBv2 Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | ELBv2 Has Tags |
| **Cloud** | AWS |
| **Category** | ELBv2 |
| **Description** | Ensure that ELBs have tags. |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_AddTags.html |
| **Recommended Action** | Modify ELB and Add tags. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/elbv2/elbv2-has-tags/step2.png"/>
3. In the "EC2 Dashboard" scroll down and look for "Load Balancers" and click on "Load Balancers" to get into "Load Balancers" dashboard.</br> <img src="/resources/aws/elbv2/elbv2-has-tags/step3.png"/>
4. Select the "Load Balancer" which needs to have tags. </br> <img src="/resources/aws/elbv2/elbv2-has-tags/step4.png"/>
5. Select the "Tags" tab from the bottom panel and Click on "Add/Edit Tags" button. </br> <img src="/resources/aws/elbv2/elbv2-has-tags/step5.png"/>
6. On "Add/Edit Tags" popup Click on "Create Tag" button and enter key-value for the tag and Click "Save".</br><img src="/resources/aws/elbv2/elbv2-has-tags/step6.png"/>
