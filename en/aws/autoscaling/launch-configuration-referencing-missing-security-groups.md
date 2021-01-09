[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / AutoScaling / Launch Configuration Referencing Missing Security Groups

## Quick Info

| | |
|-|-|
| **Plugin Title** | Launch Configuration Referencing Missing Security Groups |
| **Cloud** | AWS |
| **Category** | AutoScaling |
| **Description** | Ensures that Auto Scaling launch configurations are not utilizing missing security groups. |
| **More Info** | Auto Scaling launch configuration should utilize an active security group to ensure safety of managed instances. |
| **AWS Link** | https://docs.aws.amazon.com/autoscaling/ec2/userguide/GettingStartedTutorial.html |
| **Recommended Action** | Ensure that the launch configuration security group has not been deleted. If so, remove it from launch configurations |

## Detailed Remediation Steps




