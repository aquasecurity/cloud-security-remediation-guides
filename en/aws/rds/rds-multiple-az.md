[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / RDS / RDS Multiple AZ

## Quick Info

| | |
|-|-|
| **Plugin Title** | RDS Multiple AZ |
| **Cloud** | AWS |
| **Category** | RDS |
| **Description** | Ensures that RDS instances are created to be cross-AZ for high availability. |
| **More Info** | Creating RDS instances in a single AZ creates a single point of failure for all systems relying on that database. All RDS instances should be created in multiple AZs to ensure proper failover. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.MultiAZ.html |
| **Recommended Action** | Modify the RDS instance to enable scaling across multiple availability zones. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for RDS. </br> <img src="/resources/aws/rds/rds-multiple-az/step2.png"/>
3. Scroll down the left navigation panel and choose "Databases". </br> <img src="/resources/aws/rds/rds-multiple-az/step3.png"/>
4. Select the "Database" that needs to be verified and click on the  selected "Database" from the "DB identifier" column to access the database.</br><img src="/resources/aws/rds/rds-multiple-az/step4.png"/>
5. Click on the "Configuration" under the selected database configuration page.</br><img src="/resources/aws/rds/rds-multiple-az/step5.png"/>
6. Scroll down the "Configuration" tab and check the "Availability" section. Check the "Multi-AZ" and if its status is "No" then selected database cannot scale across multiple availability zones .</br><img src="/resources/aws/rds/rds-multiple-az/step6.png"/>
7. Select the "Database" on which automated backup needs to be enabled. Click the "Modify" button at the top to make the necessary changes.</br><img src="/resources/aws/rds/rds-multiple-az/step7.png"/>
8. Scroll down the "Modify DB Instance" page and check for "Multi-AZ deployment" under "Availability & durability".</br><img src="/resources/aws/rds/rds-multiple-az/step8.png"/>
9. On the "Multi-AZ deployment" section under "Availability & durability" select "Create a standby instance" option.</br><img src="/resources/aws/rds/rds-multiple-az/step9.png"/>
10. Scroll down the "Modify DB Instance" page and click on "Continue" button. </br><img src="/resources/aws/rds/rds-multiple-az/step10.png"/>
11. On the "Scheduling of modifications" choose "Apply immediately" so that changes will be applied as soon as possible and click on the "Modify DB Instance" button. </br><img src="/resources/aws/rds/rds-multiple-az/step11.png"/>
12. Repeat steps number 7 - 11 to enable scaling across multiple availability zones.</br>
