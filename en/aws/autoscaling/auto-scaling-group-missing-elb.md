[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / AutoScaling / Auto Scaling Group Missing ELB

## Quick Info

| | |
|-|-|
| **Plugin Title** | Auto Scaling Group Missing ELB |
| **Cloud** | AWS |
| **Category** | AutoScaling |
| **Description** | Ensures all Auto Scaling groups are referencing active load balancers. |
| **More Info** | Each Auto Scaling group with a load balancer configured should reference an active ELB. |
| **AWS Link** | https://docs.aws.amazon.com/autoscaling/ec2/userguide/attach-load-balancer-asg.html |
| **Recommended Action** | Ensure that the Auto Scaling group load balancer has not been deleted. If so, remove it from the ASG. |

## Detailed Remediation Steps




