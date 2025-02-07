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
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for RDS. </br> <img src="/resources/aws/rds/rds-publicly-accessible/step2.png"/>
3. Scroll down the left navigation panel and choose "Databases". </br> <img src="/resources/aws/rds/rds-publicly-accessible/step3.png"/>
4. Select the "Database" that needs to be verified and click on the selected "Database" from the "DB identifier" column to access the database.</br><img src="/resources/aws/rds/rds-publicly-accessible/step4.png"/>
5. Click on the "Connectivity & Security" under the selected database configuration page.</br><img src="/resources/aws/rds/rds-publicly-accessible/step5.png"/>
6. Scroll down the "Connectivity & Security" tab and check the "Security" section. Check the "Public Accessibility" and if it's "Yes" then selected database can launched into the public cloud .</br><img src="/resources/aws/rds/rds-publicly-accessible/step6.png"/>
7. Select the "Database" on which "Public Accessibility" needs to be disabled. Click the "Modify" button at the top to make the necessary changes.</br><img src="/resources/aws/rds/rds-publicly-accessible/step7.png"/>
8. Scroll down the "Modify DB Instance" page and check for "Public Access" under "Additional configuration" of "Connectivity".</br><img src="/resources/aws/rds/rds-publicly-accessible/step8.png"/>
9. On the "Public Access" section under "Connectivity" select the "Not publicly accessible" option.</br><img src="/resources/aws/rds/rds-publicly-accessible/step9.png"/>
10. Scroll down the "Modify DB Instance" page and click on "Continue" button. </br><img src="/resources/aws/rds/rds-publicly-accessible/step10.png"/>
11. On the "Scheduling of modifications" choose "Apply immediately" so that it will make the above changes as soon as possible, and then click on the "Modify DB Instance" button. </br><img src="/resources/aws/rds/rds-publicly-accessible/step11.png"/>
12. Repeat steps number 7 - 11 to remove the public access from all other RDS instances .</br>
