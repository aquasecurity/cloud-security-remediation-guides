[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# Google / Dataproc / Dataproc Cluster Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | Dataproc Cluster Encryption |
| **Cloud** | Google |
| **Category** | Dataproc |
| **Description** | Ensure that Dataproc clusters have encryption enabled using desired protection level. |
| **More Info** | By default, all dataproc clusters are encrypted using Google-managed keys. To have better control over how your dataproc clusters are encrypted, you can use Customer-Managed Keys (CMKs). |
| **Google Link** | https://cloud.google.com/dataproc/docs/concepts/configuring-clusters/customer-managed-encryption |
| **Recommended Action** | Ensure that all dataproc clusters have desired encryption level. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose "Dataproc" to select the "Clusters" option. </br> <img src="/resources/google/dataproc/dataproc-cluster-encryption/step2.png">
3. On the "Clusters" page, select the cluster which needs to be verified whether it has CMK encryption enabled or not by clicking on its name.</br> <img src="/resources/google/dataproc/dataproc-cluster-encryption/step3.png"/>
4. On the "Cluster details" page, click on the "Configuration" tab. </br> <img src="/resources/google/dataproc/dataproc-cluster-encryption/step4.png"/>
5. Scroll down and check the value of "Encryption type". If "Encryption type" is set to "Google-managed key" then the cluster is not encrypted using CMK.</br> <img src="/resources/google/dataproc/dataproc-cluster-encryption/step5.png"/>
6. Repeat step number 2 - 5 to verify other "Clusters" in the project.</br>
7. Navigate to "Dataproc" and choose "Clusters", and click on the name of the "Cluster" that needs to have CMK encryption enabled to go to the "Cluster details" page.</br> <img src="/resources/google/dataproc/dataproc-cluster-encryption/step3.png"/>
8. From the "Cluster details" page, collect all the configuration information for the cluster.</br>
9. Go back to the "Clusters" page and click the "Create Cluster" button at top.</br> <img src="/resources/google/dataproc/dataproc-cluster-encryption/step9.png"/>
10. On the "Create Cluster" page, add all the configuration information of the old cluster and then click on "Manage Security" tab on the left-side.</br> <img src="/resources/google/dataproc/dataproc-cluster-encryption/step10.png"/>
11. Under "Encryption", check the button next to "Customer-managed encryption key (CMEK)" and then from the "Select a customer-managed key" dropdown, choose the CMK you want to use for cluster encryption.</br> <img src="/resources/google/dataproc/dataproc-cluster-encryption/step11.png"/>
12. Click the "Create" button on left side to create a new dataproc cluster with CMK encyrption enabled.</br> <img src="/resources/google/dataproc/dataproc-cluster-encryption/step12.png"/>
13. Once the new "Cluster" is created, delete the old cluster by clicking on the checkbox next to its name and then clicking on the "Delete" button at the top.</br> <img src="/resources/google/dataproc/dataproc-cluster-encryption/step13.png"/>
14. Confirm the deleteion by clicking on the "Confirm" button in the "Confirm deletion" popup.</br> <img src="/resources/google/dataproc/dataproc-cluster-encryption/step14.png"/>
15. Repeat steps number 7 - 14 to recreate all the Dataproc "Clusters" in the project with Customer Managed Encryption keys.</br>

