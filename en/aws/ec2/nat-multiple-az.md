[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / NAT Multiple AZ

## Quick Info

| | |
|-|-|
| **Plugin Title** | NAT Multiple AZ |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures managed NAT instances exist in at least 2 AZs for availability purposes |
| **More Info** | Creating NAT instances in a single AZ creates a single point of failure for all systems in the VPC. All managed NAT instances should be created in multiple AZs to ensure proper failover. |
| **AWS Link** | http://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/vpc-nat-gateway.html |
| **Recommended Action** | Launch managed NAT instances in multiple AZs. |

## Detailed Remediation Steps

