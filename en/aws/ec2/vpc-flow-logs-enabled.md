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
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for VPC. </br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step2.png"/>
3. Scroll down the left navigation panel and choose "Your VPCs" under "Virtual Private Cloud". </br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step3.png"/>
4. Select the "VPC" that needs to be verified for "VPC Flow Logs". </br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step4.png"/>
5. Scroll down the bottom dashboard panel and choose "Flow Logs" tab. If there are no flow logs then "No flow logs found in this Region" message will be displayed. </br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step5.png"/>
6. Repeat steps number 2 - 6 to verify whether "Flow Logs" are enabled or not for other VPCs in the remaining regions. </br>
7. Navigate to "Your VPCs" in the left navigation panel, select the VPC and click on the "Flow Logs" tab in the bottom dashboard panel.</br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step7.png"/>
8. Click on the "Create flow log" button to create the "VPC Flow Logs". </br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step8.png"/>
9. In the "Create flow log" dialog box select the "Filter" that describes the type of traffic to be logged and select the "Maximum aggregation interval".</br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step9.png"/>
10. Select the destination to which the flow log data is to be published from the options. If the "S3 bucket" is selected then provide the "S3 Bucket ARN" in which the flow log is to be published. Also select the "Log Record Format" & "Log File Format" along with the "Partition logs by time" and click on the "Create flow log" button at the bottom. </br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step10.png"/>
11. If destination for the "flow log data" is selected as "Send to CloudWatch Logs" then enter the log destination in "Destination log group" which is the name of the "Amazon CloudWatch Logs" log group to which the flow log is published. Select the "IAM role" that has permission to publish to the "Amazon CloudWatch Logs" log group and specify the "Log record format". Then click on the "Create flow log" button to make the necessary changes.</br> <img src="/resources/aws/ec2/vpc-flow-logs-enabled/step11.png"/>
12. Repeat steps number 7 - 11 to enable VPC flow logs for other "VPCs" in the region.</br>
