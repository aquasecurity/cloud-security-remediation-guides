[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Redshift / Redshift Encryption Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Redshift Encryption Enabled |
| **Cloud** | AWS |
| **Category** | Redshift |
| **Description** | Ensures at-rest encryption is setup for Redshift clusters |
| **More Info** | AWS provides at-read encryption for Redshift clusters which should be enabled to ensure the integrity of data stored within the cluster. |
| **AWS Link** | http://docs.aws.amazon.com/redshift/latest/mgmt/working-with-db-encryption.html |
| **Recommended Action** | Redshift does not currently allow modifications to encryption after the cluster has been launched, so a new cluster will need to be created with encryption enabled. |

## Detailed Remediation Steps

