[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Transfer / Transfer Logging Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Transfer Logging Enabled |
| **Cloud** | AWS |
| **Category** | Transfer |
| **Description** | Ensures AWS Transfer servers have CloudWatch logging enabled. |
| **More Info** | AWS Transfer servers can log activity to CloudWatch if a proper IAM service role is provided. This role should be configured for all servers to ensure proper access logging. |
| **AWS Link** | https://docs.aws.amazon.com/transfer/latest/userguide/monitoring.html |
| **Recommended Action** | Provide a valid IAM service role for AWS Transfer servers. |

## Detailed Remediation Steps

