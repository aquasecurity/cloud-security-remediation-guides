[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / RDS / RDS Restorable

## Quick Info

| | |
|-|-|
| **Plugin Title** | RDS Restorable |
| **Cloud** | AWS |
| **Category** | RDS |
| **Description** | Ensures RDS instances can be restored to a recent point |
| **More Info** | AWS will maintain a point to which the database can be restored. This point should not drift too far into the past, or else the risk of irrecoverable data loss may occur. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_PIT.html |
| **Recommended Action** | Ensure the instance is running and configured properly. If the time drifts too far, consider opening a support ticket with AWS. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for RDS. </br> <img src="/resources/aws/rds/rds-restorable/step2.png"/>
3. Scroll down the left navigation panel and choose "Databases". </br> <img src="/resources/aws/rds/rds-restorable/step3.png"/>
4. Select the "Database" that needs to be verified and click on the  selected "Databse" from the "DB identifier" column to access the database.</br><img src="/resources/aws/rds/rds-restorable/step4.png"/>
5. Click on the "Maintenance & backups" under the selected database configuration page.</br><img src="/resources/aws/rds/rds-restorable/step5.png"/>
6. Scroll down the "Maintenance & backups" tab and check the "Backup".Check the "Automated backups" and "Latest restore time". If "Automated backups" are enabled and "Latest restore time" is showing the latest timestamp than the selected database can be restored. </br><img src="/resources/aws/rds/rds-restorable/step6.png"/>
7. If the "Latest restore time" is showing timestamp from past than click on the "Support" at the top right panel and click on "Support Center".</br><img src="/resources/aws/rds/rds-restorable/step7.png"/>
8. Click on the "Create case" button under "My support cases".</br><img src="/resources/aws/rds/rds-restorable/step8.png"/>
9. Click on the "Technical Support" and open a support ticket with AWS for RDS.</br><img src="/resources/aws/rds/rds-restorable/step9.png"/>
