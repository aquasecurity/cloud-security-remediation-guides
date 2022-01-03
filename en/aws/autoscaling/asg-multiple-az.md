[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / AutoScaling / ASG Multiple AZ

## Quick Info

| | |
|-|-|
| **Plugin Title** | ASG Multiple AZ |
| **Cloud** | AWS |
| **Category** | AutoScaling |
| **Description** | Ensures that ASGs are created to be cross-AZ for high availability. |
| **More Info** | ASGs can easily be configured to allow instances to launch in multiple availability zones. This ensures that the ASG can continue to scale, even when AWS is experiencing downtime in one or more zones. |
| **AWS Link** | http://docs.aws.amazon.com/autoscaling/latest/userguide/AutoScalingGroup.html |
| **Recommended Action** | Modify the autoscaling instance to enable scaling across multiple availability zones. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console and Search for "EC2" to reach EC2 dashboard.</br><img src="/resources/aws/autoscaling/asg-multiple-az/step1.png"/>
2. In the left navigation panel, scroll down and choose Auto Scaling Groups option under "Auto Scaling".</br> <img src="/resources/aws/autoscaling/asg-multiple-az/step2.png"/>
3. Select the Auto Scaling Group(s) that needs to be modified.</br> <img src="/resources/aws/autoscaling/asg-multiple-az/step3.png"/>
4. Scroll down to select the "Details" tab and check the Availability Zone(s). </br> <img src="/resources/aws/autoscaling/asg-multiple-az/step4.png"/>
5. If Availability Zone(s) value under "Network" is set to a single availability zone (e.g. us-east-1b), it cannot launch instances to multiple Availability Zone(s) hence if one Availability Zone becomes unavailable, Amazon EC2 Auto Scaling cannot launch instances in another one to one.</br><img src="/resources/aws/autoscaling/asg-multiple-az/step5.png"/>
6. Select the Auto Scaling Group and click on "Edit".</br><img src="/resources/aws/autoscaling/asg-multiple-az/step6.png"/>
7. In the Edit Web-ASG page  scroll down to "Network" and from the dropdown select the desired multiple availibility zones.</br><img src="/resources/aws/autoscaling/asg-multiple-az/step7.png"/>
8. Edit the Subnet(s) and add the Subnet(s) to make the Auto Scaling Group available to Multiple Availability Zone(s).</br><img src="/resources/aws/autoscaling/asg-multiple-az/step6.png"/>
9. Save the changes. Go to "Details" option and now Availability Zone(s) have multiple regions and subnets as well.</br><img src="/resources/aws/autoscaling/asg-multiple-az/step7.png"/>
10. Repeat the steps number 2 and 3 to establish any other Auto Scaling Group hosted in multiple Availability Zone(s) or not. 
