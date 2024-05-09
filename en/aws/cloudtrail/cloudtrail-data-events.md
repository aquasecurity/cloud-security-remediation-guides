[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudTrail / CloudTrail Data Events

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudTrail Data Events |
| **Cloud** | AWS |
| **Category** | CloudTrail |
| **Description** | Ensure Data events are included into Amazon CloudTrail trails configuration. |
| **More Info** | AWS CloudTrail trails should be configured to enable Data Events in order to log S3 object-level API operations. |
| **AWS Link** | https://docs.aws.amazon.com/awscloudtrail/latest/userguide/logging-data-events-with-cloudtrail.html |
| **Recommended Action** | Update CloudTrail to enable data events. |

## Detailed Remediation Steps
1. Sign in to the AWS Management Console.

2. Navigate to Amazon [CloudTrail console](https://console.aws.amazon.com/cloudtrail/).

3. In the navigation panel, under CloudTrail, choose Trails.</br><img src="/resources/aws/cloudtrail/cloudtrail-data-events/step3.png"/>

4. Click on the name of the Amazon CloudTrail trail that you want to examine.

5. In the Data events section, if the following message is displayed: Data event collection is not configured for this trail, the selected Amazon CloudTrail trail is not configured to capture operations performed on or in an AWS cloud resource.</br><img src="/resources/aws/cloudtrail/cloudtrail-data-events/step5.png"/>

6. To enable Data Events click on Edit. </br><img src="/resources/aws/cloudtrail/cloudtrail-data-events/step6.png"/>
7. Click the checkbox Data Events. </br><img src="/resources/aws/cloudtrail/cloudtrail-data-events/step7.png"/>
8. Choose the source of the data events to log.</br><img src="/resources/aws/cloudtrail/cloudtrail-data-events/step8.png"/>
9. Choose the log Selector Template. 
10. Click Save changes. 
11. Repeat steps no. 4 to 10 for each Amazon CloudTrail trail created for your AWS account.

**Note:** Additional charges apply for data events. For more information, see [AWS CloudTrail Pricing](https://aws.amazon.com/cloudtrail/pricing/).

**Best practice** create a lifecycle configuration for your AWS CloudTrail data event bucket. Configure the lifecycle configuration to periodically remove log files after the period of time you believe you need to audit them. Doing so reduces the amount of data that Athena analyzes for each query. For more information, see [Setting a lifecycle configuration on a bucket](https://docs.aws.amazon.com/AmazonS3/latest/userguide/how-to-set-lifecycle-configuration-intro.html).
