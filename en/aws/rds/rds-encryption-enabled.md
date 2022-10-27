[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / RDS / RDS Encryption Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | RDS Encryption Enabled |
| **Cloud** | AWS |
| **Category** | RDS |
| **Description** | Ensures at-rest encryption is setup for RDS instances |
| **More Info** | AWS provides at-read encryption for RDS instances which should be enabled to ensure the integrity of data stored within the databases. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Overview.Encryption.html |
| **Recommended Action** | RDS does not currently allow modifications to encryption after the instance has been launched, so a new instance will need to be created with encryption enabled. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for RDS. </br> <img src="/resources/aws/rds/rds-encryption-enabled/step2.png"/>
3. Scroll down the left navigation panel and choose "Databases". </br> <img src="/resources/aws/rds/rds-encryption-enabled/step3.png"/>
4. Select the "Database" that needs to be verified and click on the  selected "Database" from the "DB identifier" column to access the database.</br><img src="/resources/aws/rds/rds-encryption-enabled/step4.png"/>
5. Click on the "Configuration" under the selected database configuration page.</br><img src="/resources/aws/rds/rds-encryption-enabled/step5.png"/>
6. Scroll down the "Configuration" tab and check the "Storage" section.Check the "Encryption" and if it's "Not Enabled" then encryption is not setup for selected RDS instance.</br><img src="/resources/aws/rds/rds-encryption-enabled/step6.png"/>
7. Select the "Database" on which "Encryption" needs to be enabled.</br><img src="/resources/aws/rds/rds-encryption-enabled/step7.png"/>
8. Click on the "Actions" button at the top panel and click on "Take snapshot". </br><img src="/resources/aws/rds/rds-encryption-enabled/step8.png"/>
9. On "Take DB snapshot" page provide a "Snapshot name" which will act as an identifier for the "DB Snapshot" and click on "Take Snapshot" button.</br><img src="/resources/aws/rds/rds-encryption-enabled/step9.png"/>
10. Select the new created "Snapshot" and click on the "Actions" button at the top menu and click on the "Copy Snapshot" option.</br><img src="/resources/aws/rds/rds-encryption-enabled/step10.png"/>
11. Under the "Copy snapshot" configuration page select the "Destination Region" and provide the "New DB Snapshot Identifier" for the new snapshot. </br><img src="/resources/aws/rds/rds-encryption-enabled/step11.png"/>
12. Scroll down the "Copy snapshot" configuration page and click on "Enable encryption" under Encryption section. Select the "AWS KMS Key" from dropdown menu and click on the "Copy Snapshot" button.</br><img src="/resources/aws/rds/rds-encryption-enabled/step12.png"/>
13. Select the new created "Snapshot" and click on the "Actions" button at the top menu and click on the "Restore Snapshot" option.</br><img src="/resources/aws/rds/rds-encryption-enabled/step13.png"/>
14. On "Restore snapshot" configuration page review all the configuration settings and provide a unique name to the "DB Instance Identifier" under "Settings".</br><img src="/resources/aws/rds/rds-encryption-enabled/step14.png"/>
15. Scroll down and click on the "Restore DB Instance" button. </br><img src="/resources/aws/rds/rds-encryption-enabled/step15.png"/>
16. Update the "Database Endpoint" as soon as the new instance provisioning process is completed and the database instance is available. </br><img src="/resources/aws/rds/rds-encryption-enabled/step16.png"/>
17. Remove the unencrypted database instance by selecting the database and clicking on the "Actions" button at the top menu and clicking on the "Delete" button under "Delete" panel. </br><img src="/resources/aws/rds/rds-encryption-enabled/step17.png"/>
18. Repeat step 7 to 17 for all other RDS databases. 
