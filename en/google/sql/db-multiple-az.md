[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / SQL / DB Multiple Az

## Quick Info

| | |
|-|-|
| **Plugin Title** | DB Multiple Az |
| **Cloud** | GOOGLE |
| **Category** | SQL |
| **Description** | Ensures that SQL instances have a failover replica to be cross-AZ for high availability. |
| **More Info** | Creating SQL instances in with a single AZ creates a single point of failure for all systems relying on that database. All SQL instances should be created in multiple AZs to ensure proper failover. |
| **GOOGLE Link** | https://cloud.google.com/sql/docs/mysql/instance-settings |
| **Recommended Action** | 1. Enter the SQL category of the Google Console. 2. Select the instance. 3. Select the Replicas tab. 4. Select Create Failover Replica and follow the prompts. |

## Detailed Remediation Steps

