[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / RDS / RDS Publicly Accessible

## Quick Info

| | |
|-|-|
| **Plugin Title** | RDS Publicly Accessible |
| **Cloud** | AWS |
| **Category** | RDS |
| **Description** | Ensures RDS instances are not launched into the public cloud |
| **More Info** | Unless there is a specific business requirement, RDS instances should not have a public endpoint and should be accessed from within a VPC only. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_VPC.html |
| **Recommended Action** | Remove the public endpoint from the RDS instance |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for RDS. </br> <img src="/resources/aws/rds/rds-publicly-accessible/step2.png"/>
3. Scroll down the left navigation panel and choose "Databases". </br> <img src="/resources/aws/rds/rds-publicly-accessible/step3.png"/>
4. Select the "Database" that needs to be verified and click on the  selected "Databse" from the "DB identifier" column to access the database.</br><img src="/resources/aws/rds/rds-publicly-accessible/step4.png"/>
5. Click on the "Connectivity & Security" under the selected database configuration page.</br><img src="/resources/aws/rds/rds-publicly-accessible/step5.png"/>
6. Scroll down the "Connectivity & Security" tab and check the "Security" section.Check the "Public Accessibility" and if it's "Yes" then selected database can launched into the public cloud .</br><img src="/resources/aws/rds/rds-publicly-accessible/step6.png"/>
7. Repeat steps number 2 - 6 to check other RDS instances. </br>
8. Select the "Database" on which "Public Accessibility" needs to be disable. Click the "Modify" button at the top to make the necessary changes.</br><img src="/resources/aws/rds/rds-publicly-accessible/step8.png"/>
9. Scroll down the "Modify DB Instance" page and check for "Public Accessibility" under "Network & Security".</br><img src="/resources/aws/rds/rds-publicly-accessible/step9.png"/>
10. On the "Public Accessibility" section under "Network & Security" click on the "No" button.</br><img src="/resources/aws/rds/rds-publicly-accessible/step10.png"/>
11. Scroll down the "Modify DB Instance" page and click on "Continue" button. </br><img src="/resources/aws/rds/rds-publicly-accessible/step11.png"/>
12. On the "Scheduling of modifications" choose "Apply immediately" so that it will made the above changes applied as soon as possible and click on the "Modify DB Instance" button. </br><img src="/resources/aws/rds/rds-publicly-accessible/step12.png"/>
13. Repeat steps number 8 - 12 to remove the public endpoint from the RDS instances .</br>
