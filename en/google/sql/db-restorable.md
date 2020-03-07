[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / DB Restorable

## Quick Info

| | |
|-|-|
| **Plugin Title** | DB Restorable |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures SQL instances can be restored to a recent point |
| **More Info** | Google will maintain a point to which the database can be restored. This point should not drift too far into the past, or else the risk of irrecoverable data loss may occur. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/mysql/instance-settings |
| **Recommended Action** | Ensure all database instances are configured with automatic backups and can be restored to a recent point with binary logging enabled. |

## Detailed Remediation Steps
1. Log in to the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "SQL" option under the "Storage." </br> <img src="/resources/google/sql/db-restorable/step2.png"/>
3. On the "SQL" page , click on the "Instance ID" as a link option to select the "SQL" instance.</br> <img src="/resources/google/sql/db-restorable/step3.png"/>
4. On the "SQL" page, click on the "Overview" under the "MASTER INSTANCE."</br> <img src="/resources/google/sql/db-restorable/step4.png"/>
5. On the "Overview" page, check whether "Enable binary logging (required for replication and earlier position point-in-time recovery)" is showing enabled or disabled. If "Enable binary logging" is showing "Disabled" then the selected SQL instance cannot maintain a point to which the database can be restored.</br> <img src="/resources/google/sql/db-restorable/step5.png"/>
6. Repeat steps number 2 - 5 to check other SQL instance in the account.</br> 
7. Navigate to the "SQL" option under the "Storage", choose the "SQL Instance" and click on the "Edit" button at the top.</br> <img src="/resources/google/sql/db-restorable/step7.png"/>
8. On the "Edit instance" page, scroll down and click on the "Auto backups and high availability" under the "Configuration options."</br> <img src="/resources/google/sql/db-restorable/step8.png"/>
9. On the "db-automated-backups" tab, click on the checkbox next to "Enable binary logging."</br> <img src="/resources/google/sql/db-restorable/step9.png"/>
10. Click on the "Save" button to make the changes.</br> <img src="/resources/google/sql/db-restorable/step10.png"/>
11. Repeat steps number 7 - 10 to ensure all database instances are configured with automatic backups and can be restored to a recent point with binary logging enabled.</br>

