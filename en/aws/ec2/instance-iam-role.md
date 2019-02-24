[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Instance IAM Role

## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance IAM Role |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures EC2 instances are using an IAM role instead of hard-coded AWS credentials |
| **More Info** | IAM roles should be assigned to all instances to enable them to access AWS resources. Using an IAM role is more secure than hard-coding AWS access keys into application code. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/iam-roles-for-amazon-ec2.html |
| **Recommended Action** | Attach an IAM role to the EC2 instance |

## Detailed Remediation Steps

