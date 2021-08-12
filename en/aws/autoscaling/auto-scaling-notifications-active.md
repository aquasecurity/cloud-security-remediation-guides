[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / AutoScaling / Auto Scaling Notifications Active

## Quick Info

| | |
|-|-|
| **Plugin Title** | Auto Scaling Notifications Active |
| **Cloud** | AWS |
| **Category** | AutoScaling |
| **Description** | Ensures auto scaling groups have notifications active. |
| **More Info** | Notifications can be sent to an SNS endpoint when scaling actions occur, which should be set to ensure all scaling activity is recorded. |
| **AWS Link** | https://docs.aws.amazon.com/autoscaling/ec2/userguide/ASGettingNotifications.html |
| **Recommended Action** | Add a notification endpoint to the auto scaling group. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/autoscaling/auto-scaling-notifications-active/step2.png"/>
3. In the EC2 Management console, scroll down and click on the "Auto Scaling groups" at the bottom.</br> <img src="/resources/aws/autoscaling/auto-scaling-notifications-active/step3.png"/>
4. On the "Auto Scaling groups" page, select the Auto Scaling group which needs to be verified for the active notifications.</br> <img src="/resources/aws/autoscaling/auto-scaling-notifications-active/step4.png"/>
5. On the "Auto Scaling group", click on the "Activity" tab and check if any notifications are currently specified or not.If "No notifications are currently specified" is showing it means the selected group don't have any active notifications.</br> <img src="/resources/aws/autoscaling/auto-scaling-notifications-active/step5.png"/>
6. Repeat steps number 2 - 5 to check other Auto Scaling groups in the account.</br> 
7. Navigate to the EC2 console using the link https://console.aws.amazon.com/ec2/ .</br>
8. Scroll down the EC2 console page, select the Auto Scaling groups and select the Auto Scaling group which needs to have notifications enabled.</br> <img src="/resources/aws/autoscaling/auto-scaling-notifications-active/step8.png"/>
9. Click on the "Activity" tab, select the "Create notification" option at the top right corner.</br> <img src="/resources/aws/autoscaling/auto-scaling-notifications-active/step9.png"/>
10. On the "Create notification" tab, click on the "Create a topic" option if you don't have the SNS topic already configured.</br> <img src="/resources/aws/autoscaling/auto-scaling-notifications-active/step10.png"/>
11. Enter the "Send a notification to" and email address details to whom you want to send the notifications and click on the "Create" button.</br> <img src="/resources/aws/autoscaling/auto-scaling-notifications-active/step11.png"/>
12. Repeat steps number 7 - 11 to add a notification endpoint to the Auto Scaling group.</br> 

