[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudWatch / VPC Flow Logs Metric Alarm

## Quick Info

| | |
|-|-|
| **Plugin Title** | VPC Flow Logs Metric Alarm |
| **Cloud** | AWS |
| **Category** | CloudWatch |
| **Description** | Ensure that an AWS CloudWatch alarm exists and configured for metric filter attached with VPC flow logs CloudWatch group. |
| **More Info** | A metric alarm watches a single CloudWatch metric or the result of a math expression based on CloudWatch metrics. The alarm performs one or more actions based on the value of the metric or expression relative to a threshold over a number of time periods. The action can be sending a notification to an Amazon SNS topic. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/AlarmThatSendsEmail.html |
| **Recommended Action** | Create a CloudWatch group, attached metric filter to log VPC flow logs changes and create an CloudWatch alarm for the metric filter. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for VPC. Ensure flow logs are created for your required VPCs. If not, choose Create Flow Log and select Cloudwatch as the destination. </br> <img src="/resources/aws/cloudwatch/step1.png"/>
3. Open Cloudwatch from AWS console. Select the VPC flow log - log group if exists already or create one. </br> <img src="/resources/aws/cloudwatch/step2.png"/>
4. Create metric filters based on the selected log group. </br>  </br> <img src="/resources/aws/cloudwatch/step3.png"/>
5. Set up alarms based on the metrics. </br>  </br> <img src="/resources/aws/cloudwatch/step4.png"/>
