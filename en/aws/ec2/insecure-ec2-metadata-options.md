[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Insecure EC2 Metadata Options

## Quick Info

| | |
|-|-|
| **Plugin Title** | Insecure EC2 Metadata Options |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures EC2 instance metadata is updated to require HttpTokens or disable HttpEndpoint |
| **More Info** | The new EC2 metadata service prevents SSRF attack escalations from accessing the sensitive instance metadata endpoints. |
| **AWS Link** | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-metadata.html#configuring-instance-metadata-service |
| **Recommended Action** | Update instance metadata options to use IMDSv2 |

## Detailed Remediation Steps




