[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Kubernetes / Legacy Authorization Disabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Legacy Authorization Disabled |
| **Cloud** | GOOGLE |
| **Category** | Kubernetes |
| **Description** | Ensure legacy authorization is set to disabled on Kubernetes clusters |
| **More Info** | The legacy authorizer in Kubernetes grants broad, statically defined permissions. |
| **GOOGLE Link** | https://cloud.google.com/kubernetes-engine/docs/how-to/hardening-your-cluster |
| **Recommended Action** | Disable legacy authorization on all clusters. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Kubernetes Engine" option under the "Compute" and select the "Clusters." </br> <img src="/resources/google/kubernetes/legacy-authorization-disabled/step2.png"/>
3. On the "Kubernetes clusters" page , click on the "Name" as a link option to select the cluster.</br> <img src="/resources/google/kubernetes/legacy-authorization-disabled/step3.png"/>
4. On the "Clusters" page, click on the "Edit" button at the top.</br> <img src="/resources/google/kubernetes/legacy-authorization-disabled/step4.png"/>
5. Scroll down the "Clusters - Edit" page and check whether "Legacy Authorisation" is enabled or disabled. If it's set to enabled then it's not as per the best recommended method.</br> <img src="/resources/google/kubernetes/legacy-authorization-disabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Clusters" in the account.</br>
7. Navigate to the "Kubernetes Engine" option under the "Compute", choose the "Clusters" and click on the "Edit" button at the top.</br> <img src="/resources/google/kubernetes/legacy-authorization-disabled/step7.png"/>
8. On the "Clusters - Edit" page, scroll down and choose the "Disabled" option from the dropdown menu next to "Legacy Authorisation."</br> <img src="/resources/google/kubernetes/legacy-authorization-disabled/step8.png"/>
9. Click on the "Save" button to make the changes.</br> <img src="/resources/google/kubernetes/legacy-authorization-disabled/step9.png"/>
10. Repeat steps number 7 - 9 to disable legacy authorization on all clusters.</br>


