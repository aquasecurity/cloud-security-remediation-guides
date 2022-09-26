[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / IAM Users Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | IAM Users Has Tags |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensure IAM users have tags |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/IAM/latest/UserGuide/id_tags_users.html |
| **Recommended Action** | Modify IAM User and add tags |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for IAM. </br><img src="/resources/aws/iam/iam-users-has-tags/step2.png"/>
3. On the left navigation panel and choose "Users". </br><img src="/resources/aws/iam/iam-users-has-tags/step3.png"/>
4. Select the User from the User List for which you want to add tags. </br><img src="/resources/aws/iam/iam-users-has-tags/step4.png"/>
5. On the "Summary" page Choose "Tags" from the navigation panel. Under the "Tags" tab Click on "Add tags" button.</br><img src="/resources/aws/iam/iam-users-has-tags/step5.png"/>
6. Enter the key and value for the tag and Click "Save changes" at the botton of the page.</br><img src="/resources/aws/iam/iam-users-has-tags/step6.png"/>

