[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudTrail / CloudTrail Management Events

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudTrail Management Events |
| **Cloud** | AWS |
| **Category** | CloudTrail |
| **Description** | Ensures that AWS CloudTrail trails are configured to log management events. |
| **More Info** | AWS CloudTrail trails should be configured to log management events to record management operations that are performed on resources in your AWS account. |
| **AWS Link** | https://docs.aws.amazon.com/awscloudtrail/latest/userguide/logging-management-events-with-cloudtrail.html |
| **Recommended Action** | Update CloudTrail to enable management events logging. |

## Detailed Remediation Steps
1. Sign in to the AWS Management Console.
2. Navigate to Amazon [CloudTrail console](https://console.aws.amazon.com/cloudtrail/).
3. In the navigation panel, under CloudTrail, choose Trails.</br><img src="/resources/aws/cloudtrail/cloudtrail-management-events/step3.png"/>
4. Click on the name of the Amazon CloudTrail trail that you want to Edit.
5. In the Management events section, if the following message is displayed: Management events are not configured for this trail, the selected Amazon CloudTrail trail is not configured to capture management operations performed on your AWS resources.</br><img src="/resources/aws/cloudtrail/cloudtrail-management-events/step5.png"/>
6. To update the trail configuration settings click Edit from the Management events section to edit the .</br><img src="/resources/aws/cloudtrail/cloudtrail-management-events/step5.png"/>
7. In the Edit trail configuration page, do the following steps:
   a. In the Events section, under Event type select Management events.</br><img src="/resources/aws/cloudtrail/cloudtrail-management-events/step7a.png"/>
   b. In the Management events section, under API activity, choose if you want your trail or event data store to log Read events, Write events, or both. <br />
   **Read:**<br />
   Read-only events include API operations that read your resources, but don't make changes. For example, read-only events include the Amazon EC2 DescribeSecurityGroups and DescribeSubnets API operations. These operations return only information about your Amazon EC2 resources and don't change your configurations.
   **Write:**<br />
   Write to record write-only events (i.e. API operations that change or might change your AWS resources, such as RunInstances and TerminateInstances API operations). Choose both Read and Write if you want your CloudTrail trail to log all API operations.
   </br><img src="/resources/aws/cloudtrail/cloudtrail-management-events/step7b.png"/>
   c. (Optional) Choose Exclude AWS KMS events to filter AWS Key Management Service (AWS KMS) events out of your trail or event data store. The default setting is to include all AWS KMS events.
   d. (Optional) Choose Exclude Amazon RDS Data API events to filter Amazon Relational Database Service Data API events out of your trail or event data store. The default setting is to include all Amazon RDS Data API events.
8. Click Save changes when you are finished.
9. Repeat steps no. 4 – 8 for each Amazon CloudTrail trail that you want to update in your AWS account.