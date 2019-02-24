[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Excessive Security Groups

## Quick Info

| | |
|-|-|
| **Plugin Title** | Excessive Security Groups |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determine if there are an excessive number of security groups in the account |
| **More Info** | Keeping the number of security groups to a minimum helps reduce the attack surface of an account. Rather than creating new groups with the same rules for each project, common rules should be grouped under the same security groups. For example, instead of adding port 22 from a known IP to every group, create a single "SSH" security group which can be used on multiple instances. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/authorizing-access-to-an-instance.html |
| **Recommended Action** | Limit the number of security groups to prevent accidental authorizations |

## Detailed Remediation Steps

