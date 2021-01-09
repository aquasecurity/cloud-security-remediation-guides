[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / RDS / SQL Server TLS Version

## Quick Info

| | |
|-|-|
| **Plugin Title** | SQL Server TLS Version |
| **Cloud** | AWS |
| **Category** | RDS |
| **Description** | Ensures RDS SQL Servers do not allow outdated TLS certificate versions |
| **More Info** | TLS 1.2 or higher should be used for all TLS connections to RDS. A parameter group can be used to enforce this connection type. |
| **AWS Link** | https://aws.amazon.com/about-aws/whats-new/2020/07/amazon-rds-for-sql-server-supports-disabling-old-versions-of-tls-and-ciphers/ |
| **Recommended Action** | Create a parameter group that contains the TLS version restriction and limit access to TLS 1.2 or higher |

## Detailed Remediation Steps




