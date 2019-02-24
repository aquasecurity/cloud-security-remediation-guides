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

