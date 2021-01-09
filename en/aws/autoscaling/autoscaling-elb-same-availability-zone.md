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




