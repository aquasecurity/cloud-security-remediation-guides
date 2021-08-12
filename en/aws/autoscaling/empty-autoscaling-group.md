[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / AutoScaling / Empty AutoScaling Group

## Quick Info

| | |
|-|-|
| **Plugin Title** | Empty AutoScaling Group |
| **Cloud** | AWS |
| **Category** | AutoScaling |
| **Description** | Ensures all autoscaling groups contain at least 1 instance. |
| **More Info** | AutoScaling groups that are no longer in use should be deleted to prevent accidental use. |
| **AWS Link** | https://docs.aws.amazon.com/autoscaling/ec2/userguide/AutoScalingGroup.html |
| **Recommended Action** | Delete the unused AutoScaling group. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/autoscaling/empty-autoscaling-group/step2.png"/>
3. In the EC2 Management console, scroll down and click on the "Auto Scaling groups" at the bottom.</br> <img src="/resources/aws/autoscaling/empty-autoscaling-group/step3.png"/>
4. On the "Auto Scaling groups" page, select the auto scaling group which needs to be verified whether autoscaling groups contain at least 1 instance or not.</br> <img src="/resources/aws/autoscaling/empty-autoscaling-group/step4.png"/>
5. On the "Auto Scaling group" page, scroll down and check if there is any instance running under the "Instances". If no instance is running, delete the selected Auto Scaling group.</br> <img src="/resources/aws/autoscaling/empty-autoscaling-group/step5.png"/>
6. Repeat steps number 2 - 5 to check other groups in the account.</br>
7. Navigate to the EC2 console using the link https://console.aws.amazon.com/ec2/ .</br>
8. Select the Auto Scaling group from the left navigation panel and select the Auto Scaling group without any active isntance.</br> <img src="/resources/aws/autoscaling/empty-autoscaling-group/step8.png"/>
9. Click on the "Delete" button at the top after selecting the Auto Scaling group.</br> <img src="/resources/aws/autoscaling/empty-autoscaling-group/step9.png"/>
10. On the "Delete Auto Scaling groups" tab, type delete in the box for the confirmation and click on the "Delete" button to make the changes.</br> <img src="/resources/aws/autoscaling/empty-autoscaling-group/step10.png"/>
11. Repeat steps number 7 - 10 to delete the unused Auto Scaling group.</br>

