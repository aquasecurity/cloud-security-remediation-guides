[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / IAM Roles Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | IAM Roles Has Tags |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensure that AWS IAM Roles have tags associated. |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/IAM/latest/UserGuide/id_tags.html |
| **Recommended Action** | Modify IAM Role and add tags |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for IAM. </br><img src="/resources/aws/iam/iam-roles-has-tags/step2.png"/>
3. On the left navigation panel and choose "Roles". </br><img src="/resources/aws/iam/iam-roles-has-tags/step3.png"/>
4. Select the Role from the Roles List for which you want to add tags. </br><img src="/resources/aws/iam/iam-roles-has-tags/step4.png"/>
5. On the "Summary" page Choose "Tags" from the navigation panel. Under the "Tags" tab Click on "Manage Tags" button.</br><img src="/resources/aws/iam/iam-roles-has-tags/step5.png"/>
6. On "Manage Tags" page click on Click on "Add Tags" then enter key value pair for the tags and Click "Save changes" button.</br><img src="/resources/aws/iam/iam-roles-has-tags/step6.png"/>

