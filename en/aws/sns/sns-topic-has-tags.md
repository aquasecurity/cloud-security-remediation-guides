[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / SNS / SNS Topic Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | SNS Topic Has Tags |
| **Cloud** | AWS |
| **Category** | SNS |
| **Description** | Ensure that Amazon SNS Topics have tags associated. |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/sns/latest/dg/sns-tags.html |
| **Recommended Action** | Modify SNS topics and add tags. |

## Detailed Remediation Steps

1. Log into the AWS Management Console.
2. Select the "Services" option and search for SNS. </br> <img src="/resources/aws/sns/sns-topic-has-tags/step2.png"/>
3. Choose "Topic" from left navigation panel.</br> <img src="/resources/aws/sns/sns-topic-has-tags/step3.png"/>
4. On "Topics" page choose the topic for which needs to have tags by clicking on the "Name".</br> <img src="/resources/aws/sns/sns-topic-has-tags/step4.png"/>
5. On the "Topics" details page Choose the "Tags" tab from bottom of the page and Click "Add Tags" button.</br> <img src="/resources/aws/sns/sns-topic-has-tags/step5.png"/>
6. On Edit topic page scroll down to the tags section. Expand the tags section enter the key-value pair for the tags and click "Save changes" button at the bottom of the page. </br> <img src="/resources/aws/sns/sns-topic-has-tags/step5.png"/>



