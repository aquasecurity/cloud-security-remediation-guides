[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / Any Host Root Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Any Host Root Access |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures SQL instances root user cannot be accessed from any host |
| **More Info** | Root access for SQL instance should only be allowed from whitelisted IPs to ensure secure access only from trusted entities. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/mysql/create-manage-users |
| **Recommended Action** | Ensure that root access for SQL instances are not allowed from any host. |

## Detailed Remediation Steps
1. Log in to the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "SQL" option under the "Storage." </br> <img src="/resources/google/sql/any-host-root-access/step2.png"/>
3. On the "SQL" page , click on the "Instance ID" as a link option to select the "SQL" instance.</br> <img src="/resources/google/sql/any-host-root-access/step3.png"/>
4. On the "SQL" page, click on the "Connections" under the "MASTER INSTANCE."</br> <img src="/resources/google/sql/any-host-root-access/step4.png"/>
5. On the "Conenctions" page, scroll down the Conenctivity and check whether any "Authorised Network" is configured or it's open to the "Public IP" to access for everyone.</br> <img src="/resources/google/sql/any-host-root-access/step5.png"/>
6. Repeat steps number 2 - 5 to check other "SQL Instances" in the account.
7. Navigate to the "SQL" option under the "Storage", choose the "SQL Instance" and click on the "Edit" button at the top.</br> <img src="/resources/google/sql/any-host-root-access/step7.png"/>
8. On the "Edit instance" page, scroll down and click on the "Conenctivity" under the "Configuration options."</br> <img src="/resources/google/sql/any-host-root-access/step8.png"/>
9. On the "Conenctivity" tab, click on the "Add network" option under the "Public IP."</br> <img src="/resources/google/sql/any-host-root-access/step9.png"/>
10. On the "New Network" tab, enter the "Network Name" and "IP Details" as per the requirement and click on the "Done" button to make the changes.</br> <img src="/resources/google/sql/any-host-root-access/step10.png"/>
11. Click on the "Save" button at the bottom of the page to make the changes.</br> <img src="/resources/google/sql/any-host-root-access/step11.png"/>
12. Repeat steps number 7 - 11 to ensure that root access for SQL instances are not allowed from any host.</br>
