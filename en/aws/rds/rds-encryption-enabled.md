[![CloudSploit](https://cloudsploit.com/img/logo-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / RDS / RDS Encryption Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | RDS Encryption Enabled |
| **Cloud** | AWS |
| **Category** | RDS |
| **Description** | Ensures at-rest encryption is setup for RDS instances |
| **More Info** | AWS provides at-read encryption for RDS instances which should be enabled to ensure the integrity of data stored within the databases. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Overview.Encryption.html |
| **Recommended Action** | RDS does not currently allow modifications to encryption after the instance has been launched, so a new instance will need to be created with encryption enabled. |

## Detailed Remediation Steps

