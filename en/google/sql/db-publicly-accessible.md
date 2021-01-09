[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / DB Publicly Accessible

## Quick Info

| | |
|-|-|
| **Plugin Title** | DB Publicly Accessible |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures that SQL instances do not allow public access |
| **More Info** | Unless there is a specific business requirement, SQL instances should not have a public endpoint and should only be accessed from within a VPC. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/mysql/authorize-networks |
| **Recommended Action** | Ensure that SQL instances are configured to prohibit traffic from the public 0.0.0.0 global IP address. |

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


