[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / EBS Encryption Enabled By Default

## Quick Info

| | |
|-|-|
| **Plugin Title** | EBS Encryption Enabled By Default |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensure the setting for encryption by default is enabled |
| **More Info** | AWS account should be configured to enable encryption for new EBS volumes and snapshots for all regions |
| **AWS Link** | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSEncryption.html#encryption-by-default |
| **Recommended Action** | Enable EBS Encryption by Default |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> 
3. On Amazon EC2 console,from the navigation bar, select the Region. </br>
4. From the navigation pane, select EC2 Dashboard. </br>
5. In the upper-right corner of the page, choose Account Attributes, EBS encryption. </br>
6. Choose Manage. </br>
7. Select Enable. You keep the AWS managed key with the alias alias/aws/ebs created on your behalf as the default encryption key, or choose a symmetric customer managed encryption key. </br>
8. Choose Update EBS encryption. </br>