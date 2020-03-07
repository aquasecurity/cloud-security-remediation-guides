[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / DB Publicly Accessible

## Quick Info

| | |
|-|-|
| **Plugin Title** | DB Publicly Accessible |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures that SQL instances have a failover replica to be cross-AZ for high availability. |
| **More Info** | Creating SQL instances in with a single AZ creates a single point of failure for all systems relying on that database. All SQL instances should be created in multiple AZs to ensure proper failover. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/mysql/instance-settings |
| **Recommended Action** | 1. Enter the SQL category of the Google Console. 2. Select the instance. 3. Select the Replicas tab. 4. Select Create Failover Replica and follow the prompts. |

## Detailed Remediation Steps
1. Log in to the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "SQL" option under the "Storage." </br> <img src="/resources/google/sql/db-publicly-accessible/step2.png"/>
3. On the "SQL" page , click on the "Instance ID" as a link option to select the "SQL" instance.</br> <img src="/resources/google/sql/db-publicly-accessible/step3.png"/>
4. On the "SQL" page, click on the "Replicas" under the "MASTER INSTANCE."</br> <img src="/resources/google/sql/db-publicly-accessible/step4.png"/>
5. On the "Replicas" page, check is there any "Relica" is there or not. Creating SQL instances in with a single AZ creates a single point of failure for all systems </br> <img src="/resources/google/sql/db-publicly-accessible/step5.png"/>
6. Repeat steps number 2 - 5 to check other SQL instance in the account.</br> 
7. Navigate to the "SQL" option under the "Storage", choose the "SQL Instance".</br> <img src="/resources/google/sql/db-publicly-accessible/step7.png"/>
8. Click on the "Replicas" from the left panel and click on the "Create read replica" button at the bottom.</br> <img src="/resources/google/sql/db-publicly-accessible/step8.png"/>
9. On the "Create read replica", click on the checkbox next to "Automate backups", "Enable binary logging" and click on the "Continue" button.</br> <img src="/resources/google/sql/db-publicly-accessible/step9.png"/>
10. Once you click on the "Continue" button, "Changes require restart" tab will open and click on the "SAVE AND RESTART" option.</br> <img src="/resources/google/sql/db-publicly-accessible/step10.png"/>
11. Click on the "Create" button to make the changes.</br> <img src="/resources/google/sql/db-publicly-accessible/step11.png"/>
12. Repeat steps number 7 - 11 to ensure all SQL instances should be created in multiple AZs to ensure proper failover.  


