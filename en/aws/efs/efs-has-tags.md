[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EFS / EFS Encryption Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | EFS Has Tags |
| **Cloud** | AWS |
| **Category** | EFS |
| **Description** | Ensure EFS File systems have tags |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/efs/latest/ug/manage-fs-tags.html |
| **Recommended Action** | Add new tags for efs file system. |

## Detailed Remediation Steps

1. Log into the AWS Management Console.
2. Select the "Services" option and search for EFS.</br> <img src="/resources/aws/efs/efs-has-tags/step2.png"/>
3. Select the EFS file system for which you want to add tags.".</br> <img src="/resources/aws/efs/efs-has-tags/step3.png"/>
4. Select the "Tags" tab from navigation pane on the page.</br> <img src="/resources/aws/efs/efs-has-tags/step4.png"/>
5. Click on "Manage Tag" button.</br> <img src="/resources/aws/efs/efs-has-tags/step5.png"/>
6. On the popup modal click on "Add Tag". Then enter the key and value for your tag and click Save.</br> <img src="/resources/aws/efs/efs-has-tags/step6.png"/>


