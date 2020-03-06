[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / Database SSL Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Database SSL Enabled |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures SQL databases have SSL enabled |
| **More Info** | Enabling SSL ensures that the sensitive data being transferred from the database is encrypted. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/mysql/instance-settings |
| **Recommended Action** | Ensure that SSL is enabled on all SQL databases. |

## Detailed Remediation Steps
1. Log in to the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "SQL" option under the "Storage." </br> <img src="/resources/google/sql/database-ssl-enabled/step2.png"/>
3. On the "SQL" page , click on the "Instance ID" as a link option to select the "SQL" instance.</br> <img src="/resources/google/sql/database-ssl-enabled/step3.png"/>
4. On the "SQL" page, click on the "Connections" under the "MASTER INSTANCE."</br> <img src="/resources/google/sql/database-ssl-enabled/step4.png"/>
5. On the "Conenctions" page, scroll down the page and check the "SSL Connections" whether they are allowed for unsecured or only secured connections. If it's showing "Unsecured connections are allowed to connect to this instance" then it's not as per the recommended guidelines.</br> <img src="/resources/google/sql/database-ssl-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to check other "SQL Instances" in the account.
7. Navigate to the "SQL" option under the "Storage", choose the "SQL Instance" and click on the "Edit" button at the top.</br> <img src="/resources/google/sql/database-ssl-enabled/step7.png"/>
8. On the "Edit instance" page, scroll down and click on the "Allow only SSL connections" button under the "SSL connections."</br> <img src="/resources/google/sql/database-ssl-enabled/step8.png"/>
9. Click on the "Create new certificate" button under the "Configure SSL server certificates" to create a new set of SSL certificates if needed.</br> <img src="/resources/google/sql/database-ssl-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to ensure that SSL is enabled on all SQL databases.</br>

