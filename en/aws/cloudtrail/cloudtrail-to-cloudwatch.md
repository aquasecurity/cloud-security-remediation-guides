[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudTrail / CloudTrail To CloudWatch

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudTrail To CloudWatch |
| **Cloud** | AWS |
| **Category** | CloudTrail |
| **Description** | Ensures CloudTrail logs are being properly delivered to CloudWatch |
| **More Info** | Sending CloudTrail logs to CloudWatch enables easy integration with AWS CloudWatch alerts, as well as an additional backup log storage location. |
| **AWS Link** | http://docs.aws.amazon.com/awscloudtrail/latest/userguide/send-cloudtrail-events-to-cloudwatch-logs.html |
| **Recommended Action** | Enable CloudTrail CloudWatch integration for all regions |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "CloudTrail".</br>![Step 2](/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step2.png "Step 2 - Services")
3. In the "Dashboard" panel click on "View trails" button.</br> ![Step 3](/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step3.png "Step 3 - Trails")
4. Select the "trail" that needs to be verified under "Name" column.</br>![Step 4](/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step4.png "Step 4 - Name")
5. Scroll down and under the "CloudWatch Logs" option check for any log groups configuration. If no log groups are there than "CloudWatch" is not enabled for the selected trail. </br>![Step 5](/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step5.png "Step 5 - CloudWatch Logs")
6. Click on the "Configure" button under the "CloudWatch Logs" section to configure log groups. </br>![Step 6](/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step6.png "Step 6 - Configure")
7. In "New or existing log group" enter a name for log group and click on "Continue". </br>![Step 7](/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step7.png "Step 7 - Name")
8. Create a new "IAM Role" to deliver CloudTrail events to CloudWatch Logs log group. Role Name is defined on it's own once we click on new "IAM Role". </br>![Step 8](/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step8.png "Step 8 - IAM Role")
9. Click on "View Policy Document" to verify the "CloudTrail_CloudWatchLogs_Role".</br> ![Step 9](/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step9.png "Step 9 - Policy")
10. Click "Allow" to save the changes. "CloudTrail CloudWatch" is now enabled for the selected trail.</br>![Step 10](/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step10.png "Step 10 - Allow")
