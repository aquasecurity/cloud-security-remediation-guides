[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / AutoScaling / Suspended AutoScaling Groups

## Quick Info

| | |
|-|-|
| **Plugin Title** | Suspended AutoScaling Groups |
| **Cloud** | AWS |
| **Category** | AutoScaling |
| **Description** | Ensures that there are no Amazon AutoScaling groups with suspended processes. |
| **More Info** | AutoScaling groups should not have any suspended processes to avoid disrupting the AutoScaling workflow. |
| **AWS Link** | https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-suspend-resume-processes.html |
| **Recommended Action** | Update the AutoScaling group to resume the suspended processes. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/autoscaling/suspended-autoscaling-groups/step2.png"/>
3. In the EC2 Management console, scroll down and click on the "Auto Scaling groups" at the bottom.</br> <img src="/resources/aws/autoscaling/suspended-autoscaling-groups/step3.png"/>
4. On the "Auto Scaling groups" page, select the auto scaling group which needs to be verified that there are no Amazon AutoScaling groups with suspended processes.</br> <img src="/resources/aws/autoscaling/suspended-autoscaling-groups/step4.png"/>
5. On the "Auto Scaling groups" page, scroll down and under "Advanced configurations" check for Suspended Processes configuration attribute and if the value is set to one or more auto scaling processes such as Launch, Terminate, HealthCheck then the selected Auto Scaling group has one or more suspended processes.</br> <img src="/resources/aws/autoscaling/suspended-autoscaling-groups/step5.png"/>
6. Repeat steps number 2 - 5 to check other Auto Scaling groups in the account.</br>
7. Navigate to the EC2 console using the link https://console.aws.amazon.com/ec2/ .</br>
8. Scroll down the EC2 console page, select the "Auto Scaling group" from the left navigation panel and select the Auto scaling group in which one have to resume the suspended processes.</br> <img src="/resources/aws/autoscaling/suspended-autoscaling-groups/step8.png"/>
9. On the "Auto Scaling groups" page, scroll down and under "Advanced configurations" click on the "Edit" button.</br> <img src="/resources/aws/autoscaling/suspended-autoscaling-groups/step9.png"/>
10. Remove the suspended auto scaling process available within Suspended Processes box by click on X option. Click on the Update button at the bottom to make the changes.</br> <img src="/resources/aws/autoscaling/suspended-autoscaling-groups/step10.png"/>
11. Repeat steps number 7 - 10 to update the AutoScaling group to resume the suspended processes.</br>



