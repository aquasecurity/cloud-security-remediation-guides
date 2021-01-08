[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Kubernetes / Monitoring Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Monitoring Enabled |
| **Cloud** | GOOGLE |
| **Category** | Kubernetes |
| **Description** | Ensures all Kubernetes clusters have monitoring enabled |
| **More Info** | Kubernetes supports monitoring through Stackdriver. |
| **GOOGLE Link** | https://cloud.google.com/monitoring/kubernetes-engine/ |
| **Recommended Action** | Ensure monitoring is enabled on all Kubernetes clusters. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Kubernetes Engine" option under the "Compute" and select the "Clusters." </br> <img src="/resources/google/kubernetes/monitoring-enabled/step2.png"/>
3. On the "Kubernetes clusters" page , click on the "Name" as a link option to select the cluster.</br> <img src="/resources/google/kubernetes/monitoring-enabled/step3.png"/>
4. On the "Clusters" page, click on the "Edit" button at the top.</br> <img src="/resources/google/kubernetes/monitoring-enabled/step4.png"/>
5. Scroll down the "Clusters - Edit" page and check whether "Stackdriver Kubernetes Engine Monitoring" is enabled or disabled. If it's set to disabled then it's not as per the best recommended method.</br> <img src="/resources/google/kubernetes/monitoring-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Clusters" in the account.</br>
7. Navigate to the "Kubernetes Engine" option under the "Compute", choose the "Clusters" and click on the "Edit" button at the top.</br> <img src="/resources/google/kubernetes/monitoring-enabled/step7.png"/>
8. On the "Clusters - Edit" page, scroll down and choose the "System and workload logging and monitoring" option from the dropdown menu next to "Stackdriver Kubernetes Engine Monitoring."</br> <img src="/resources/google/kubernetes/monitoring-enabled/step8.png"/>
9. Click on the "Save" button to make the changes.</br> <img src="/resources/google/kubernetes/monitoring-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to ensure that monitoring is enabled on all Kubernetes clusters.</br>

