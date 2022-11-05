[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ECR / ECR Repository Tag Immutability

## Quick Info

| | |
|-|-|
| **Plugin Title** | ECR Repository Has Tags |
| **Cloud** | AWS |
| **Category** | ECR |
| **Description** | Ensure that ECR repositories have tags |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonECR/latest/userguide/ecr-using-tags.html |
| **Recommended Action** | Modify ECR repository and add tags |

## Detailed Remediation Steps

1. Log into the AWS Management Console.
2. Select the "Services" option and search for ECR. </br> <img src="/resources/aws/ecr/ecr-repository-has-tags/step2.png"/>
3. Click on  "Repositories" from navigation panel on the left.</br> <img src="/resources/aws/ecr/ecr-repository-has-tags/step3.png"/>
4. Select the "Repository" which needs to have tags by clicking on name. </br> <img src="/resources/aws/ecr/ecr-repository-has-tags/step4.png"/>
5. On repository details page Click on "Repository tags" from navigation panel on the left.</br> <img src="/resources/aws/ecr/ecr-repository-has-tags/step5.png"/>
6. On "Repository tags" page Click on "Add tags" button.</br> <img src="/resources/aws/ecr/ecr-repository-has-tags/step6.png"/>
7. On "Edit Repository tags" page Click on "Add tags" button enter the key value pair and Click "Save".</br> <img src="/resources/aws/ecr/ecr-repository-has-tags/step7.png"/>


