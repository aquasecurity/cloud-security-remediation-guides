[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / VM Instances Least Privilege

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Instances Least Privilege |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensures that instances are not configured to use the default service account with full access to all cloud APIs |
| **More Info** | To support the principle of least privilege and prevent potential privilege escalation, it is recommended that instances are not assigned to the default service account, Compute Engine default service account with a scope allowing full access to all cloud APIs. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/access/create-enable-service-accounts-for-instances |
| **Recommended Action** | For all instances, if the default service account is used, ensure full access to all cloud APIs is not configured. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Compute Engine" to select the "VM Instances" option. </br> <img src="/resources/google/compute/vm-instances-least-privilege/step2.png"/>
3. On the "VM Instances" page, select the VM instance which needs to be verified. </br> <img src="/resources/google/compute/vm-instances-least-privilege/step3.png"/>
4. On the "VM instance details" page, scroll down and check "Cloud API access scopes" and see if the "Default service account" is used or not.</br> <img src="/resources/google/compute/vm-instances-least-privilege/step4.png"/>
5. Repeat steps number 2 - 4 to verify other VM instances in the network.</br>
6. Navigate to "Compute Engine", choose the "VM instances" and select the "VM instance" which needs to ensures that instances are not configured to use the default service account with full access to all cloud APIs.</br> <img src="/resources/google/compute/vm-instances-least-privilege/step6.png"/>
7. On the "VM instance details" page, select the "Edit" button at the top.</br> <img src="/resources/google/compute/vm-instances-least-privilege/step7.png"/>
8. On the "VM instance details - Edit page", scroll down the page and check the "Cloud API access scopes" and make sure "full access to all cloud APIs is not configured." </br> <img src="/resources/google/compute/vm-instances-least-privilege/step8.png"/>
9. Click on the "Save" button to make the changes.</br> <img src="/resources/google/compute/vm-instances-least-privilege/step9.png"/>
10. If "full access to all cloud APIs is configured", we need to create a replica of that instance and need to launch the "Instance" with restricting "Cloud APIs" access.</br> 
11. Repeat steps number 6 - 10  to ensure if the default service account is used, ensure full access to all cloud APIs is not configured.</br>

