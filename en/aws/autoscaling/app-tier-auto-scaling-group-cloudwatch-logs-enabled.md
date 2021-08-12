[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / AutoScaling / App-Tier Auto Scaling Group CloudWatch Logs Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | App-Tier Auto Scaling Group CloudWatch Logs Enabled |
| **Cloud** | AWS |
| **Category** | AutoScaling |
| **Description** | Ensures that App-Tier Auto Scaling Groups are using CloudWatch logs agent. |
| **More Info** | EC2 instance available within app-tier Auto Scaling Group (ASG) should use an AWS CloudWatch Logs agent to monitor, store and access log files. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/Install-CloudWatch-Agent.html |
| **Recommended Action** | Update app-tier Auto Scaling Group to use CloudWatch Logs agent |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/autoscaling/app-tier-auto-scaling-group-cloudwatch-logs-enabled/step2.png"/>
3. In the EC2 Management console, scroll down and click on the "Auto Scaling groups" at the bottom.</br> <img src="/resources/aws/autoscaling/app-tier-auto-scaling-group-cloudwatch-logs-enabled/step3.png"/>
4. On the "Auto Scaling groups" page, select the Auto Scaling group which needs to be verified whether CloudWatch logs are enabled or not.</br> <img src="/resources/aws/autoscaling/app-tier-auto-scaling-group-cloudwatch-logs-enabled/step4.png"/>
5. On the "Auto Scaling group", click on the "Monitoring" tab and check if "Auto Scaling group metrics collection" is enabled or not.</br> <img src="/resources/aws/autoscaling/app-tier-auto-scaling-group-cloudwatch-logs-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to ensure that App-Tier Auto Scaling Groups are using CloudWatch logs.</br>
7. Navigate to the EC2 console using the link https://console.aws.amazon.com/ec2/ .</br>
8. Scroll down the EC2 console page, select the Auto Scaling groups and select the Auto Scaling group which needs to have CloudWatch logs enabled.</br> <img src="/resources/aws/autoscaling/app-tier-auto-scaling-group-cloudwatch-logs-enabled/step8.png"/>
9. Click on the "Monitoring" tab, click on the "Enable" checkbox next to the Auto Scaling group metrics collection.</br> <img src="/resources/aws/autoscaling/app-tier-auto-scaling-group-cloudwatch-logs-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to update app-tier Auto Scaling Group to use CloudWatch Metrics.</br>

