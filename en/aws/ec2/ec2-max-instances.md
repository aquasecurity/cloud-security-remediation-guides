[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / EC2 Max Instances

## Quick Info

| | |
|-|-|
| **Plugin Title** | EC2 Max Instances |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures the total number of EC2 instances does not exceed a set threshold. |
| **More Info** | The number of running EC2 instances should be carefully audited, especially in unused regions, to ensure only approved applications are consuming compute resources. Many compromised AWS accounts see large numbers of EC2 instances launched. |
| **AWS Link** | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/monitoring_ec2.html |
| **Recommended Action** | Ensure that the number of running EC2 instances matches the expected count. If instances are launched above the threshold, investigate to ensure they are legitimate. |

## Detailed Remediation Steps

