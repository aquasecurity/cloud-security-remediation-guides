[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Unused Elastic Network Interfaces

## Quick Info

| | |
|-|-|
| **Plugin Title** | Unused Elastic Network Interfaces |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures that unused AWS Elastic Network Interfaces (ENIs) are removed |
| **More Info** | Unused AWS ENIs should be removed to follow best practices and to avoid reaching the service limit |
| **AWS Link** | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-eni.html |
| **Recommended Action** | Delete the unused AWS Elastic Network Interfaces |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> 
3. In the navigation pane, choose Network Interfaces. </br>
4. Select the checkbox for the network the unused interface you need to delete, and then choose Actions, Delete. </br>
5. When prompted for confirmation, choose Delete. </br>