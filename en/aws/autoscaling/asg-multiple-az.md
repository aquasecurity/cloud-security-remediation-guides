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
1. Log into the AWS Management Console and choose the desired region (US-East) where Auto Scaling Group is hosted.
2. In the left navigation panel, scroll down and choose Auto Scaling Group(s) option and select the ASG(s) that needs to be delve into.
3. Select the Details tab and check the Availability Zone(s). If Availability Zone(s) value is set to a single Availability Zone(s) (e.g. us-east-1b), it cannot launch Instances to multiple Availabilty Zone(s) hence if one Availability Zone becomes unavailable, Amazon EC2 Auto Scaling cannot launch instances in another one to atone.

## Corrective Steps
1. Select the Auto Scaling Group and go to Actions Option.
2. Select the option to Edit the configuration and choose Launch Configuration Option.
3. Edit the Subnet(s) and add the Subnet(s) to make Auto Scaling Group available to Multiple Availabilty Zone(s).
4. Save the Changes. Go to Details option again and now Availability Zone(s) have multiple regions and subnets as well.
5. Repeat the steps number 2 and 3 to establish any other Auto Scaling Group hosted in multiple Availability Zone(s) or not. 
