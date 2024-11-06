[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / IAM Role Policy Unused Services
## Quick Info

| | |
|-|-|
| **Plugin Title** | IAM Role Policy Unused Services |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensure that IAM role policies are scoped properly as to not provide access to unused AWS services. |
| **More Info** | IAM role policies should only contain actions for resource types which are being used in your account i.e. dynamodb:ListTables permission should only be given when there are DynamoDB tables to adhere to security best practices and to follow principal of least-privilege. |
| **AWS Link** | https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html |
| **Recommended Action** | Ensure that all IAM roles are scoped to specific services and resource types. |

## Detailed Remediation Steps