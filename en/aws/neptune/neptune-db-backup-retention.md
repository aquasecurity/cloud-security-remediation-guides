[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Neptune / Neptune Database Instance Backup Retention

## Quick Info

| | |
|-|-|
| **Plugin Title** | Neptune Database Instance Backup Retention |
| **Cloud** | AWS |
| **Category** | Neptune |
| **Description** | Ensure that Neptune database instances have set a minimum backup retention period. |
| **More Info** | Neptune provides feature to retain incremental backups, which allows to quickly restore to any point within the backup retention period. Ensure that you have sufficient backup retention period configured in order to restore your data in the event of failure.  |
| **AWS Link** | https://docs.aws.amazon.com/neptune/latest/userguide/backup-restore-overview.html |
| **Recommended Action** | Modify Neptune database instance to configure sufficient backup retention period. |

## Detailed Remediation Steps 
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "Neptune" .</br> <img src="/resources/aws/neptune/neptune-db-backup-retention/step2.png"/>
3. On "Neptune Dashboard" page Click on "Clusters" from left navigation panel.</br> <img src="/resources/aws/neptune/neptune-db-backup-retention/step3.png"/>
4. On Neptune clusters list page, Click on the cluster name which needs to have deletion protection feature enabled.</br> <img src="/resources/aws/neptune/neptune-db-backup-retention/step4.png"/>
5. On Cluster details page, click on "Modify" button.</br> <img src="/resources/aws/neptune/neptune-db-backup-retention/step5.png"/>
6. Scroll to bottom of "Modify Cluster" page, and select "Show more".</br> <img src="/resources/aws/neptune/neptune-db-backup-retention/step6.png"/>
7. Scroll down and under the "Backup retention period" section select "7 days" or more than 7 days depending on your choice. </br> <img src="/resources/aws/neptune/neptune-db-backup-retention/step7.png"/> 
8. Scroll to bottom of page and click "Next" button. </br> <img src="/resources/aws/neptune/neptune-db-backup-retention/step8.png"/> 
8. Under "Scheduling of modifications" section check "Apply immediately" checkbox and, Click on "Submit" button.</br> <img src="/resources/aws/neptune/neptune-db-backup-retention/step9.png"/> 



