[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Neptune / Neptune Database Deletion Protection Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Neptune Database Deletion Protection Enabled |
| **Cloud** | AWS |
| **Category** | Neptune |
| **Description** | Ensure that AWS Neptune database instances have deletion protection feature enabled. |
| **More Info** | Enabling deletion protection feature for Amazon Neptune adds an extra layer of security, preventing accidental database deletions or deletion by an unauthorized user. A Neptune DB cluster can't be deleted while deletion protection is enabled which ensures continuous availability of data. |
| **AWS Link** | https://docs.aws.amazon.com/neptune/latest/userguide/manage-console-instances-delete.html |
| **Recommended Action** | Modify Neptune database instance and enable deletion protection. |

## Detailed Remediation Steps 
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "Neptune".</br> <img src="/resources/aws/neptune/neptune-db-deletion-protection/step2.png"/>
3. On "Neptune Dashboard" page, Click on "Clusters" from left navigation panel.</br> <img src="/resources/aws/neptune/neptune-db-deletion-protection/step3.png"/>
4. On Neptune clusters list page, Click on the cluster name which needs to apply deletion protection.</br> <img src="/resources/aws/neptune/neptune-db-deletion-protection/step4.png"/>
5. On Cluster details page, click on "Modify" button.</br> <img src="/resources/aws/neptune/neptune-db-deletion-protection/step5.png"/>
6. Scroll to bottom of "Modify Cluster" page and select "Show more".</br> <img src="/resources/aws/neptune/neptune-db-deletion-protection/step6.png"/>
7. Scroll down and under the "Deletion protection" section select the "Turn on deletion protection" checkbox and click "Next" button.</br> <img src="/resources/aws/neptune/neptune-db-deletion-protection/step7.png"/> 
8. Under "Scheduling of modifications" section check "Apply immediately" checkbox and, Click on "Submit" button.</br> <img src="/resources/aws/neptune/neptune-db-deletion-protection/step8.png"/> 
