[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / EC2 LaunchWizard Security Groups

## Quick Info

| | |
|-|-|
| **Plugin Title** | EC2 LaunchWizard Security Groups |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures security groups created by the EC2 launch wizard are not used |
| **More Info** | The EC2 launch wizard frequently creates insecure security groups that are exposed publicly. These groups should not be used and custom security groups should be created instead. |
| **AWS Link** | https://docs.aws.amazon.com/launchwizard/latest/userguide/launch-wizard-sap-security-groups.html |
| **Recommended Action** | Delete the launch wizard security group and replace it with a custom security group. |

## Detailed Remediation Steps




