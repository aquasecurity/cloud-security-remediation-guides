[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / VPC Flow Logs Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | VPC Flow Logs Enabled |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures VPC flow logs are enabled for traffic logging |
| **More Info** | VPC flow logs record all traffic flowing in to and out of a VPC. These logs are critical for auditing and review after security incidents. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/flow-logs.html |
| **Recommended Action** | Enable VPC flow logs for each VPC |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for VPC. </br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step2.png"/>
3. Scroll down the left navigation panel and choose "Your VPC" under "VPC Dashboard". </br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step3.png"/>
4. Select the "VPC" that needs to be verified for "VPC Flow Logs". </br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step4.png"/>
5. Scroll down the bottom dashboard panel and choose "Flow Logs" tab. If there are no flow logs then "You do not have any Flow Logs in this region" message will be displayed. </br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step5.png"/>
6. Repeat steps number 2 - 6 to verify "Flow Logs" are enabled or not in other VPCs in the region. </br>
7. Navigate to "VPC Dashboard" and choose "Your VPC" and click on the "Flow Logs" tab in the bottom dashboard panel.</br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step7.png"/>
8. Click on the "Create flow log" button to create the "VPC Flow Logs". </br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step8.png"/>
9. In the "Create flow log" dialog box select the "Filter" from the dropdown menu that describes the type of traffic to be logged.</br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step9.png"/>
10. Select the destination to which the flow log data is to be published from the options.If the "S3 bucket" is selected for the log data to be published than provide the "S3 Bucket ARN" which is the ARN of the Amazon S3 bucket to which the flow log is published and click on the "Create" button at the bottom. </br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step10.png"/>
11. If destination for the "flow log data" is selected as "Send to CloudWatch Logs" then enter the log destination in "Destination Group" which is the name of the "Amazon CloudWatch Logs" log group to which the flow log is published.</br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step11.png"/>
12. Select the "IAM role" that has permission to publish to the "Amazon CloudWatch Logs" log group and click on the "Create" button to make the necessary changes. </br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step12.png"/>
13. Repeat steps number 7 - 12 to enable VPC flow logs for other "VPCs" in the region.</br>
