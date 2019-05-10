[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / RDS / RDS Automated Backups

## Quick Info

| | |
|-|-|
| **Plugin Title** | RDS Automated Backups |
| **Cloud** | AWS |
| **Category** | RDS |
| **Description** | Ensures automated backups are enabled for RDS instances |
| **More Info** | AWS provides a simple method of backing up RDS instances at a regular interval. This should be enabled to provide an option for restoring data in the event of a database compromise or hardware failure. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_WorkingWithAutomatedBackups.html |
| **Recommended Action** | Enable automated backups for the RDS instance |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for RDS. </br> <img src="/resources/aws/rds/rds-automated-backups/step2.png"/>
3. Scroll down the left navigation panel and choose "Databases". </br> <img src="/resources/aws/rds/rds-automated-backups/step3.png"/>
4. Select the "Database" that needs to be verified and click on the  selected "Databse" from the "DB identifier" column to access the database.</br><img src="/resources/aws/rds/rds-automated-backups/step4.png"/>
5. Click on the "Maintenance & backups" under the selected database configuration page.</br><img src="/resources/aws/rds/rds-automated-backups/step5.png"/>
6. Scroll down the "Maintenance & backups" tab and check the "Backup".Check the "Automated backups" and if "Disabled " is showing than automated backups are not enabled for selected RDS instances.</br><img src="/resources/aws/rds/rds-automated-backups/step6.png"/>
7. Repeat steps number 2 - 6 to check other RDS instances. </br>
8. Select the "Database" on which automated backup needs to be enabled. Click the "Modify" button at the top to make the necessary changes.</br><img src="/resources/aws/rds/rds-automated-backups/step8.png"/>
9. Scroll down the "Modify DB Instance" page and check for "Backup" section.</br><img src="/resources/aws/rds/rds-automated-backups/step9.png"/>
10. On the "Backup" section under "Backup retention period" select number of days between 1 to 35. Select the "Start Time" during which the automated backups are created. </br><img src="/resources/aws/rds/rds-automated-backups/step10.png"/>
11. Scroll down the "Modify DB Instance" page and click on "Continue" button. </br><img src="/resources/aws/rds/rds-automated-backups/step11.png"/>
12. On the "Scheduling of modifications" choose "Apply immediately" so that it will made the above changes applied as soon as possible and click on the "Modify DB Instance" button. </br><img src="/resources/aws/rds/rds-automated-backups/step12.png"/>
13. Once the automated backups are enabled,the Automated Backups status should change to "Enabled".</br><img src="/resources/aws/rds/rds-automated-backups/step13.png"/>
14. Repeat steps number 8 - 13 to enable automated backups for other RDS Instances. </br>
