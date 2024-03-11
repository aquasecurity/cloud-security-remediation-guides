[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Web-Tier EC2 Instance IAM Role
## Quick Info

| | |
|-|-|
| **Plugin Title** | Web-Tier EC2 Instance IAM Role |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensure IAM roles attached with Web-Tier EC2 instances have IAM policies attached |
| **More Info** | EC2 instances should have IAM roles configured with necessary permission to access other AWS services |
| **AWS Link** | https://aws.amazon.com/blogs/security/new-attach-an-aws-iam-role-to-an-existing-amazon-ec2-instance-by-using-the-aws-cli/ |
| **Recommended Action** | Modify EC2 instances to attach IAM roles with required IAM policies |

## Detailed Remediation Steps
1. Create an IAM role. </br>
2. Attach the IAM role to an existing EC2 instance that was originally launched without an IAM role. </br>
3. Replace the attached IAM role. </br>
Note: You may attach an existing IAM role to an existing EC2 instance that was originally launched without an IAM role, in this case you don't need to create a new IAM Role.  </br>
Note: Before you can create an IAM role from the AWS CLI, you must create a trust policy. A trust policy permits AWS services such as EC2 to assume an IAM role on behalf of your application. </br>
for detailed steps refer to this link: https://aws.amazon.com/blogs/security/new-attach-an-aws-iam-role-to-an-existing-amazon-ec2-instance-by-using-the-aws-cli/ </br>