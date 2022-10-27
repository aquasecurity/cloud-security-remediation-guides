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
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for "CloudTrail".</br><img src="/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step2.png"/>
3. In the "Dashboard" panel click on the desired trail name from the list under "Trails" to get to its configuration page.</br> <img src="/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step3.png"/>
4. Scroll down and under the "CloudWatch Logs" option check for any log groups configuration. If no log groups are there than "CloudWatch" is not enabled for the selected trail. Click on the "Edit" button under the "CloudWatch Logs" section to configure log groups. </br><img src="/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step4.png"/>
5. On the Edit page select and check mark the CloudWatch Logs as "Enabled" </br><img src="/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step5.png"/>
6. In "New or existing "log group" enter a "Log group name" for log group. </br><img src="/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step6.png"/>
7. Create a new "IAM Role" or select an existing "IAM Role" to deliver CloudTrail events to CloudWatch Logs group. Role Name is defined on it's own once we click on new "IAM Role". </br><img src="/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step7.png"/>
8. Click on "Policy Document" to verify the "CloudTrail_CloudWatchLogs_Role".</br> <img src="/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step8.png"/>
9. Scroll down and click "Save changes". "CloudTrail CloudWatch" is now enabled for the selected trail.</br><img src="/resources/aws/cloudtrail/cloudtrail-to-cloudwatch/step9.png"/>
