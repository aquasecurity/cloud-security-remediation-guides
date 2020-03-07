[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / DB Multiple AZ

## Quick Info

| | |
|-|-|
| **Plugin Title** | DB Multiple AZ |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures that SQL instances have a failover replica to be cross-AZ for high availability |
| **More Info** | Creating SQL instances in with a single AZ creates a single point of failure for all systems relying on that database. All SQL instances should be created in multiple AZs to ensure proper failover. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/mysql/instance-settings |
| **Recommended Action** | Ensure that all database instances have a DB replica enabled in a secondary AZ. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "SQL" option under the "Storage." </br> <img src="/resources/google/sql/db-multiple-az/step2.png"/>
3. On the "SQL" page , click on the "Instance ID" as a link option to select the "SQL" instance.</br> <img src="/resources/google/sql/db-multiple-az/step3.png"/>
4. On the "SQL" page, scroll down and check the "Sugegsted actions" and if it's showing "Enable High availability", then the selected SQL instance is not as per the recommended guidelines of GCP.</br>
5. Repeat steps number 2 - 5 to check other SQL instance in the account.</br> 
6. Navigate to the "SQL" option under the "Storage", choose the "SQL Instance" and click on the "Edit" button at the top.</br> <img src="/resources/google/sql/db-multiple-az/step6.png"/>
7. On the "Edit instance" page, scroll down and click on the "Auto backups and high availability" under the "Configuration options."</br> <img src="/resources/google/sql/db-multiple-az/step7.png"/>
8. On the "db-automated-backups" tab, click on the checkbox next to "High Availability" under the "Availability" section.</br> <img src="/resources/google/sql/db-multiple-az/step8.png"/>
9. Click on the "Save" button to make the changes.</br> <img src="/resources/google/sql/db-multiple-az/step9.png"/>
10. Repeat steps number 6 - 9 to ensure that all database instances have a DB replica enabled in a secondary AZ.</br>
