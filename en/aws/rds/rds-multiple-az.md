[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / RDS / RDS Multiple AZ

## Quick Info

| | |
|-|-|
| **Plugin Title** | RDS Multiple AZ |
| **Cloud** | AWS |
| **Category** | RDS |
| **Description** | Ensures that RDS instances are created to be cross-AZ for high availability. |
| **More Info** | Creating RDS instances in a single AZ creates a single point of failure for all systems relying on that database. All RDS instances should be created in multiple AZs to ensure proper failover. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.MultiAZ.html |
| **Recommended Action** | Modify the RDS instance to enable scaling across multiple availability zones. |

## Detailed Remediation Steps

