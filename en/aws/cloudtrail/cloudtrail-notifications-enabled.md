[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudTrail / CloudTrail Notifications Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudTrail Notifications Enabled |
| **Cloud** | AWS |
| **Category** | CloudTrail |
| **Description** | Ensure that Amazon CloudTrail trails are using active Simple Notification Service (SNS) topics to deliver notifications. |
| **More Info** | CloudTrail trails should reference active SNS topics to notify for log files delivery to S3 buckets. Otherwise, you will lose the ability to take immediate actions based on log information. |
| **AWS Link** | https://docs.aws.amazon.com/awscloudtrail/latest/userguide/configure-sns-notifications-for-cloudtrail.html |
| **Recommended Action** | Make sure that CloudTrail trails are using active SNS topics and that SNS topics have not been deleted after trail creation. |

## Detailed Remediation Steps
1. Sign in to the AWS Management Console.
2. Navigate to Amazon [CloudTrail console](https://console.aws.amazon.com/cloudtrail/).
3. In the navigation panel, under CloudTrail, choose Trails.</br><img src="/resources/aws/cloudtrail/cloudtrail-data-events/step3.png"/>
4. Click on the name of the Amazon CloudTrail trail that you want to configure.
5. In the General details section, choose Edit and perform the following operations:</br><img src="/resources/aws/cloudtrail/cloudtrail-delivery-failing/step5.png"/>
   a.  Check Enable SNS notification delivery, to be notified each time a log is delivered to your bucket.</br><img src="/resources/aws/cloudtrail/cloudtrail-delivery-failing/step5a.png"/>
   b. Select New under Create a new SNS topic to create a new Amazon SNS topic and associate it with the selected trail.</br><img src="/resources/aws/cloudtrail/cloudtrail-delivery-failing/step5a.png"/>
   c. Provide a unique name for the new topic in the SNS topic box.
   d. Click Save changes to apply the changes. The new Amazon SNS topic will get permissions to receive notifications whenever a trail log file is delivered to the target S3 bucket.
6. Navigate to Amazon [SNS console](https://console.aws.amazon.com/sns/).
7. In the navigation panel, under Amazon SNS, choose Topics.
8. Click on the name of the SNS topic created at step no. 5, select the Subscriptions tab, and choose Create subscription.
9. On the Create subscription setup page, select Email from the Protocol dropdown list, enter the email address where you wish to receive trail log notifications in the Endpoint box. Finally, click Create subscription to apply the new subscription to the selected Amazon SNS topic.
10. To confirm your SNS subscription, use your preferred email client to open the subscription message from the AWS Notifications, then click on the appropriate link.
11. Repeat steps no. 4 – 10 for each Amazon CloudTrail trail that you want to edit in your AWS cloud account.