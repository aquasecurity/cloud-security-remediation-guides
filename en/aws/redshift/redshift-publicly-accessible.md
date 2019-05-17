[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Redshift / Redshift Publicly Accessible

## Quick Info

| | |
|-|-|
| **Plugin Title** | Redshift Publicly Accessible |
| **Cloud** | AWS |
| **Category** | Redshift |
| **Description** | Ensures Redshift clusters are not launched into the public cloud |
| **More Info** | Unless there is a specific business requirement, Redshift clusters should not have a public endpoint and should be accessed from within a VPC only. |
| **AWS Link** | http://docs.aws.amazon.com/redshift/latest/mgmt/getting-started-cluster-in-vpc.html |
| **Recommended Action** | Remove the public endpoint from the Redshift cluster |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for Redshift. </br> <img src="/resources/aws/redshift/redshift-publicly-accessible/step2.png"/>
3. Scroll down the left navigation panel and choose "Clusters". </br> <img src="/resources/aws/redshift/redshift-publicly-accessible/step3.png"/>
4. Select the "Cluster" that needs to be verified and click on its identifier(name) from the "Cluster" column.</br> <img src="/resources/aws/redshift/redshift-publicly-accessible/step4.png"/>
5. Scroll down the "Cluster" configuration page and check the "Publicly Accessible" option under the "Cluster Database Properties". If current status is set to "Yes" then the selected cluster is launched into the public cloud.</br><img src="/resources/aws/redshift/redshift-publicly-accessible/step5.png"/>
6. Repeat steps number 2 - 5 to verify other clusters. </br>
7. Select the "Cluster" on which "Public Accessibility" needs to be disable.Click on its identifier(name)from the "Cluster" column to go into "Cluster" configuration page.</br><img src="/resources/aws/redshift/redshift-publicly-accessible/step7.png"/>
8. Click on the "Cluster" dropdown button at the top menu and click on the "Modify Cluster" option.</br><img src="/resources/aws/redshift/redshift-publicly-accessible/step8.png"/>
9. On the "Modify Cluster" page select the "No" option next to "Publicly accessible" under "Cluster Settings". Click on the "Modify" button to make the necessary changes.</br> <img src="/resources/aws/redshift/redshift-publicly-accessible/step9.png"/>
10. Repeat steps number 7 - 9 to disable "Public Accessibility" for other clusters.</br> 
