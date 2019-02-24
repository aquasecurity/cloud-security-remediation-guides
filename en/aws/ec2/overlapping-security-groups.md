[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Overlapping Security Groups

## Quick Info

| | |
|-|-|
| **Plugin Title** | Overlapping Security Groups |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determine if EC2 instances have security groups that share the same rules |
| **More Info** | Overlapping security group rules make managing EC2 instance access much more difficult. If a rule is removed from one security group, the access may still remain in another, resulting in unintended access to the instance. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/authorizing-access-to-an-instance.html |
| **Recommended Action** | Structure security groups to provide a single category of access and do not duplicate rules across groups used by the same instances. |

## Detailed Remediation Steps

