[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / AutoScaling / AutoScaling ELB Same Availability Zone

## Quick Info

| | |
|-|-|
| **Plugin Title** | AutoScaling ELB Same Availability Zone |
| **Cloud** | AWS |
| **Category** | AutoScaling |
| **Description** | Ensures all autoscaling groups with attached ELBs are operating in the same availability zone. |
| **More Info** | To work properly and prevent orphaned instances, ELBs must be created in the same availability zones as the backend instances in the autoscaling group. |
| **AWS Link** | https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-add-availability-zone.html |
| **Recommended Action** | Update the ELB to use the same availability zones as the autoscaling group. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/autoscaling/autoscaling-elb-same-availability-zone/step2.png"/>
3. In the EC2 Management console, scroll down and click on the "Auto Scaling groups" at the bottom.</br> <img src="/resources/aws/autoscaling/autoscaling-elb-same-availability-zone/step3.png"/>
4. On the "Auto Scaling groups" page, select the auto scaling group which needs to be verified whether attached ELBs are operating in the same availability zone or not.</br> <img src="/resources/aws/autoscaling/autoscaling-elb-same-availability-zone/step4.png"/>
5. On the "Auto Scaling groups" page, scroll down and check the "Network" tab for "Availability Zones" for Auto Sacling Group.</br> <img src="/resources/aws/autoscaling/autoscaling-elb-same-availability-zone/step5.png"/>
6. Scroll down the page and click on the "Load balancer" attached to the Auto Scaling group, to check the Availability Zone of the Load balancer as well.</br> <img src="/resources/aws/autoscaling/autoscaling-elb-same-availability-zone/step6.png"/>
7. On the "Load balancer" page, check under the description for the Availability Zone and if the Availability Zone of the Auto Scaling group is not the same as Load balancer, please make the changes accordingly.</br> <img src="/resources/aws/autoscaling/autoscaling-elb-same-availability-zone/step7.png"/>
8. Repeat steps number 2 - 7 to check other groups in the account.</br>
9. Navigate to the EC2 console using the link https://console.aws.amazon.com/ec2/ .</br>
10. Scroll down the EC2 console page, select the Load balancer which needs to have the same Availability Zone as the Auto Scaling group.</br> <img src="/resources/aws/autoscaling/autoscaling-elb-same-availability-zone/step10.png"/>
11. Click on the "Instance" tab and click on the "Edit Availability Zones" button.</br> <img src="/resources/aws/autoscaling/autoscaling-elb-same-availability-zone/step11.png"/>
12. Select the "Availability Zone" from the Add and Remove Subnets which is the same as Auto Scaling group and click on the Save button to make the changes.</br> <img src="/resources/aws/autoscaling/autoscaling-elb-same-availability-zone/step12.png"/>
13. Repeat steps number 9 - 12 to update the ELB to use the same availability zones as the Auto Scaling group.</br>


