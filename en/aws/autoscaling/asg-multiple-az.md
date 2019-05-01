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
1. Log into the AWS Management Console and choose the desired region where the Auto Scaling Group is hosted.
2. In the left navigation panel, scroll down and choose Auto Scaling Group(s) option and select the Auto Scaling Group(s) that needs to be modified.</br>  ![Step 2](/resources/aws/autoscaling/asg-multiple-az/step2.png "Step 2 - ASG")  
3. Select the Details tab and check the Availability Zone(s). If Availability Zone(s) value is set to a single availability zone (e.g. us-east-1b), it cannot launch instances to multiple Availabilty Zone(s) hence if one Availability Zone becomes unavailable, Amazon EC2 Auto Scaling cannot launch instances in another one to atone.</br>![Step 3](/resources/aws/autoscaling/asg-multiple-az/step3.png "Step 3 - Details")  
4. Select the Auto Scaling Group and go to "Actions" Option.</br>![Step 4](/resources/aws/autoscaling/asg-multiple-az/step4.png "Step 4 - Actions") 
5. Select the option to "Edit" the configuration and choose the "Launch Configuration" Option.</br>![Step 5](/resources/aws/autoscaling/asg-multiple-az/Step5.png "Step 5 - Edit")
6. Edit the Subnet(s) and add the Subnet(s) to make the Auto Scaling Group available to Multiple Availabilty Zone(s).</br>![Step 6](/resources/aws/autoscaling/asg-multiple-az/step6.png "Step 6 - Subnet(s)")  
7. Save the changes. Go to "Details" option and now Availability Zone(s) have multiple regions and subnets as well.</br>![Step 7](/resources/aws/autoscaling/asg-multiple-az/step7.png "Step 7 - Details")  
8. Repeat the steps number 2 and 3 to establish any other Auto Scaling Group hosted in multiple Availability Zone(s) or not. 
