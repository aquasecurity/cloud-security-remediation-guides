[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Lambda / Lambda Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | Lambda Has Tags |
| **Cloud** | AWS |
| **Category** | Lambda |
| **Description** | Ensure that AWS Lambda functions have tags associated. |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/lambda/latest/dg/configuration-tags.html |
| **Recommended Action** | Modify Lambda function configurations and add new tags. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for Lambda. </br> <img src="/resources/aws/lambda/lambda-has-tags/step2.png"/>
3. Scroll down the left navigation panel and choose "Functions".</br> <img src="/resources/aws/lambda/lambda-has-tags/step3.png"/>
4. Select the Lambda function that needs to have tags.</br> <img src="/resources/aws/lambda/lambda-has-tags/step4.png"/>
5. On the "Lambda Functions" page scroll down and choose "Configuration".</br> <img src="/resources/aws/lambda/lambda-has-tags/step5.png"/>
6. Scroll down the "Configuration" tab and choose "Tags" tab in left navigation panel and Click on "Manage Tags".</br> <img src="/resources/aws/lambda/lambda-has-tags/step6.png"/>
7. On Manage tags page, click on "Add new tag" button. Enter key and value for tag then, click on "Save".</br> <img src="/resources/aws/lambda/lambda-has-tags/step7.png"/>
8. Repeat step number 4-7 to ensure tags on remaining Lambda functions.
