[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Neptune / Neptune Database Multiple AZ

## Quick Info

| | |
|-|-|
| **Plugin Title** | Neptune Database Multiple AZ |
| **Cloud** | AWS |
| **Category** | Neptune |
| **Description** | Ensure that AWS Neptune database instances are created to be cross-AZ for high availability. |
| **More Info** | Enabling Multi-AZ feature for Neptune instances boosts database reliability by automatically replicating data across multiple availability zones. This ensures continuous availability and minimal downtime for graph database deployments.  |
| **AWS Link** | https://docs.aws.amazon.com/neptune/latest/userguide/feature-overview-db-clusters.html |
| **Recommended Action** | Modify Neptune database instance to enable multi-AZ feature. |

## Detailed Remediation Steps 
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "Neptune".</br> <img src="/resources/aws/neptune/neptune-multi-az/step2.png"/>
3. On "Neptune Dashboard" page, Click on "Clusters" from left navigation panel.</br> <img src="/resources/aws/neptune/neptune-multi-az/step3.png"/>
4. On Neptune clusters list page Click on "Create Database".</br> <img src="/resources/aws/neptune/neptune-multi-az/step4.png"/>
5. On Create Database page scroll down and under "Availability and Durability" section, select the "Create read replica in different zone" checkbox.</br> <img src="/resources/aws/neptune/neptune-multi-az/step5.png"/>
6. Scroll to bottom of "Create Database" page, and click on "Create Database" button.</br> <img src="/resources/aws/neptune/neptune-multi-az/step6.png"/>
