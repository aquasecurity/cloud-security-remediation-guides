[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Neptune / Neptune Database Minor Version Upgrade

## Quick Info

| | |
|-|-|
| **Plugin Title** | Neptune Database Minor Version Upgrade |
| **Cloud** | AWS |
| **Category** | Neptune |
| **Description** | Ensures Auto Minor version upgrade is enabled on Neptune database instances. |
| **More Info** | AWS Neptune database service releases engine version upgrades regularly to introduce software features, bug fixes, security patches and performance improvements. Enabling auto minor version upgrade feature ensures that minor engine upgrades are applied automatically to the instance during the maintenance window.  |
| **AWS Link** |https://docs.aws.amazon.com/neptune/latest/userguide/cluster-maintenance.html |
| **Recommended Action** | Modify Neptune database instance and enable automatic minor version upgrades feature. |

## Detailed Remediation Steps 
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "Neptune". </br> <img src="/resources/aws/neptune/neptune-db-minor-version-upgrade/step2.png"/>
3. On "Neptune Dashboard" page, Click on "Clusters" from left navigation panel.</br> <img src="/resources/aws/neptune/neptune-db-minor-version-upgrade/step3.png"/>
4. On Neptune clusters list page Click on the cluster's instance name on which you want to enable auto minor version upgrade.</br> <img src="/resources/aws/neptune/neptune-db-minor-version-upgrade/step4.png"/>
5. On Instance details page, click on "Modify" button.</br> <img src="/resources/aws/neptune/neptune-db-minor-version-upgrade/step5.png"/>
6. Scroll to bottom of "Modify instance" page and select "Show more".</br> <img src="/resources/aws/neptune/neptune-db-minor-version-upgrade/step6.png"/>
7. Scroll down and under the "Auto minor version upgrade" select the "Turn on auto minor version upgrade" checkbox and click on "Next" button. </br> <img src="/resources/aws/neptune/neptune-db-minor-version-upgrade/step7.png"/> 
8. Under "Scheduling of modifications" section check "Apply immediately" checkbox and Click on "Submit" button.</br> <img src="/resources/aws/neptune/neptune-db-minor-version-upgrade/step8.png"/> 
