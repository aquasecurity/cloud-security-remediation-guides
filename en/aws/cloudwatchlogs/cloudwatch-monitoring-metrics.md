[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudWatchLogs / CloudWatch Monitoring Metrics

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudWatch Monitoring Metrics |
| **Cloud** | AWS |
| **Category** | CloudWatchLogs |
| **Description** | Ensures metric filters are setup for CloudWatch logs to detect security risks from CloudTrail. |
| **More Info** | Sending CloudTrail logs to CloudWatch is only useful if metrics are setup to detect risky activity from those logs. There are numerous metrics that should be used. For the exact filter patterns, please see this plugin on GitHub: https://github.com/cloudsploit/scans/blob/master/plugins/aws/cloudwatchlogs/monitoringMetrics.js |
| **AWS Link** | http://docs.aws.amazon.com/awscloudtrail/latest/userguide/send-cloudtrail-events-to-cloudwatch-logs.html |
| **Recommended Action** | Enable metric filters to detect malicious activity in CloudTrail logs sent to CloudWatch. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for CloudWatch. </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step2.png"/>
3. Scroll down the left navigation panel and choose "Alarms". </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step3.png"/>
4. On the "Alarms" page click on the "Settings" button below "Create alarm" button to open the CloudWatch dashboard. </br>  </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step4.png"/>
5. In the "Preference" tab scroll down the page and select the "Metric Name" toggle button and click on the "Confirm" button to save the changes. </br>  </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step5.png"/>
6. On the "Alarms" page check under "Metric Name" check any available alarm for the “CloudTrailEventCount” and if there is no such then the CloudTrail security threats are not monitored usinf CloudWatch.</br>  </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step6.png"/>
7. Repeat step nu,ber 2 - 6 to verify "CloudWatch Monitoring Metrics" for other regions. </br>
8. Select the "Services" option and search for "SNS" for creating a simple notification service to send notifications when "CloudWatch alarm" is triggered. </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step8.png"/>
9. On the "Amazon SNS" page scroll down the left navigation panel and choose "Topics" and click on the "Create topic" button at the extreme right.</br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step9.png"/>
10. In the "Create topic" page enter the "Name" and "Display name" for the topic and click on the "Create topic" button at the bottom. </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step10.png"/>
11. Access the newly created topic by clicking on the "Name" of the topic. </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step11.png"/>
12. Select the "Subscription" tab from the bottom dashboard and click on the "Create Subscription" button. </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step12.png"/>
13. Select the "Email" as "Protocol" from the dropdown menu and enter the email address that can receive notifications from "Amazon SNS" and click on the "Create subscription" button. </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step13.png"/>
14. Confirm the "Subscription" by clicking on the link on your email id for the "Amazon SNS" topic. </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step14.png"/>
15. Navigate to "CloudWatch" dashboard and select "Logs" from the left navigation panel. </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step15.png"/>
16. On the "Log Groups" page select the log group created for the CloudTrail trail event logs and click Create Metric Filter button at the top.</br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step16.png"/>
17. On the "Filter Patter" specify the terms or patterns to match log events to create metrics and click on the "Assign Metric" button at the bottom. </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step17.png"/>
18. On the "Create Metric Filter and Assign a Metric" page enter a name for the filter name and enter a name for "Metric Namespace" and "Metric Name" and click on the "Create Filter" button. </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step18.png"/>
19. Click on the "Create Alarm" button on the same page. </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step19.png"/>
20. On the "Specify metric and conditions" tab define the "Conditions" for threshold value and enter the threshold value and click on the "Next" button. </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step20.png"/>
21. On the "Configure actions" tab select the "Notification" ans "SNS Topic" by clicking on the "Select an existing SNS topic" and click on the "Next" button.</br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step21.png"/>
22. On the "Add a description" tab enter the "Alarm name" and "Alarm description" and click on the "Next" button. </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step22.png"/>
23. On the "Preview and create" page review the settings and click on the "Create alarm" button at the bottom. </br> <img src="/resources/aws/cloudwatchlogs/cloudwatch-monitoring-metrics/step23.png"/>
24. Repeat steps number 8 - 23 to enable metric filters to detect malicious activity in CloudTrail logs sent to CloudWatch. </br>
