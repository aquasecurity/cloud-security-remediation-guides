[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / DB Automated Backups

## Quick Info

| | |
|-|-|
| **Plugin Title** | DB Automated Backups |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures automated backups are enabled for SQL instances |
| **More Info** | Google provides a simple method of backing up SQL instances at a regular interval. This should be enabled to provide an option for restoring data in the event of a database compromise or hardware failure. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/mysql/instance-settings |
| **Recommended Action** | Ensure that all database instances are configured with automatic backups enabled. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "SQL" option under the "Storage." </br> <img src="/resources/google/sql/db-automated-backups/step2.png"/>
3. On the "SQL" page , click on the "Instance ID" as a link option to select the "SQL" instance.</br> <img src="/resources/google/sql/db-automated-backups/step3.png"/>
4. On the "SQL" page, click on the "Backups" under the "MASTER INSTANCE."</br> <img src="/resources/google/sql/db-automated-backups/step4.png"/>
5. On the "Backups" page, check whether "Automated backups" is showing enabled or disabled. If "Automated backups" is showing "Disabled" then the selected SQL instance cannot restore data in the event of a database compromise or hardware failure.</br> <img src="/resources/google/sql/db-automated-backups/step5.png"/>
6. Repeat steps number 2 - 5 to check other SQL instance in the account.</br> 
7. Navigate to the "SQL" option under the "Storage", choose the "SQL Instance" and click on the "Edit" button at the top.</br> <img src="/resources/google/sql/db-automated-backups/step7.png"/>
8. On the "Edit instance" page, scroll down and click on the "Auto backups and high availability" under the "Configuration options."</br> <img src="/resources/google/sql/db-automated-backups/step8.png"/>
9. On the "db-automated-backups" tab, click on the checkbox next to "Automate backups."</br> <img src="/resources/google/sql/db-automated-backups/step9.png"/>
10. Click on the "Save" button to make the changes.</br> <img src="/resources/google/sql/db-automated-backups/step10.png"/>
11. Repeat steps number 7 - 10 to ensure that all database instances are configured with automatic backups enabled.</br>
