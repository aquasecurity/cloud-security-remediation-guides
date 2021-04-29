[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / AutoScaling / Web-Tier Auto Scaling Group Associated ELB

## Quick Info

| | |
|-|-|
| **Plugin Title** | Web-Tier Auto Scaling Group Associated ELB |
| **Cloud** | AWS |
| **Category** | AutoScaling |
| **Description** | Ensures that Web-Tier Auto Scaling Group has an associated Elastic Load Balancer |
| **More Info** | Web-Tier Auto Scaling groups should have an ELB associated to distribute incoming traffic across EC2 instances. |
| **AWS Link** | https://docs.aws.amazon.com/autoscaling/ec2/userguide/attach-load-balancer-asg.html |
| **Recommended Action** | Update Web-Tier Auto Scaling group to associate ELB to distribute incoming traffic. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/autoscaling/web-tier-auto-scaling-group-associated-elb/step2.png"/>
3. In the EC2 Management console, scroll down and click on the "Auto Scaling groups" at the bottom.</br> <img src="/resources/aws/autoscaling/web-tier-auto-scaling-group-associated-elb/step3.png"/>
4. On the "Auto Scaling groups" page, select the auto scaling group which needs to be verified an associated Elastic Load Balancer .</br>  <img src="/resources/aws/autoscaling/web-tier-auto-scaling-group-associated-elb/step4.png"/>
5. On the "Auto Scaling groups" page, scroll down and check if there is any Load balancer is attached to the "Auto Scaling group" under the "Load balancing."</br> <img src="/resources/aws/autoscaling/web-tier-auto-scaling-group-associated-elb/step5.png"/>
6. Repeat steps number 2 - 5 to check other Auto Scaling groups in the account.</br>
7. Navigate to the EC2 console using the link https://console.aws.amazon.com/ec2/ .</br>
8. Scroll down the EC2 console page, select the Auto Scaling groups and select the Auto Scaling group which needs to have Elastic Load balancer attached.</br> <img src="/resources/aws/autoscaling/web-tier-auto-scaling-group-associated-elb/step8.png"/>
9. Scroll down the "Auto Scaling groups" page, click on the "Edit" button under the "Load balancing" tab.</br> <img src="/resources/aws/autoscaling/web-tier-auto-scaling-group-associated-elb/step9.png"/>
10. On the "Load balancing" page, select the type of "Load balancer" as per the requirements and the "Load balancer" from the dropdown and click on the "Update" button at the bottom to make the changes.</br> <img src="/resources/aws/autoscaling/web-tier-auto-scaling-group-associated-elb/step10.png"/>
11. Repeat steps number 7 - 10 to update Web-Tier Auto Scaling group to associate ELB to distribute incoming traffic.</br>



