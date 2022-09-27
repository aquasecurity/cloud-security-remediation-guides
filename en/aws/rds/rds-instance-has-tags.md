[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / RDS / RDS Instance Have Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | RDS Instance Have Tags |
| **Cloud** | AWS |
| **Category** | RDS |
| **Description** | Ensure RDS instances have tags |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_Tagging.html |
| **Recommended Action** | Modify the RDS instance to add tags |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for RDS. </br> <img src="/resources/aws/rds/rds-instance-has-tags/step2.png"/>
3. Scroll down the left navigation panel and choose "Databases". </br> <img src="/resources/aws/rds/rds-instance-has-tags/step3.png"/>
4. Select the "Database" that needs to have tags and click on the  selected "Databse" from the "DB identifier" column to access the database.</br><img src="/resources/aws/rds/rds-instance-has-tags/step4.png"/>
5. On Database details Choose "Tags" from navigation panel in middle of page.</br><img src="/resources/aws/rds/rds-instance-has-tags/step5.png"/>
6. Under "Tags" tab and Click on "Add Tags" button</br><img src="/resources/aws/rds/rds-instance-has-tags/step6.png"/>
7. On the pop up screen enter key, value pair for tag and Click on "Add" button.</br><img src="/resources/aws/rds/rds-instance-has-tags/step7.png"/>