[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / VM Instances with No Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Instances with No Access |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that instances are not configured to use the default service account with full access to all Cloud APIs. |
| **More Info** | To support principle of least privileges and prevent potential privilege escalation it is recommended that instances are not assigned to default service account Compute Engine default service account with Scope Allow full access to all Cloud APIs. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/access/create-enable-service-accounts-for-instances |
| **Recommended Action** | In Service Account Section, ensure Allow full access to all Cloud APIs is not selected if selecting the default service account. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Compute Engine" to select the "VM Instances" option. </br> <img src="/resources/google/compute/vm-instances-with-no-access/step2.png"/>
3. On the "VM Instances" page, select the VM instance which needs to be verified. </br> <img src="/resources/google/compute/vm-instances-with-no-access/step3.png"/>
4. On the "VM instance details" page, scroll down and check "Cloud API access scopes" and if "Allow full access to all Cloud APIs" is selected then it's not as per the best practices of GCP.</br> <img src="/resources/google/compute/vm-instances-with-no-access/step4.png"/>
5. Repeat steps number 2 - 4 to verify other VM instances in the network.</br>
6. Navigate to "Compute Engine", choose the "VM instances" and select the "VM instance" which needs to disabled "full access to all Cloud APIs" for VM instance.</br> <img src="/resources/google/compute/vm-instances-with-no-access/step6.png"/>
7. On the "VM instance details" page, select the "CREATE SIMILAR" button at the top.</br> <img src="/resources/google/compute/vm-instances-with-no-access/step7.png"/>
8. Enter the "Name" of the instance, Region, Choose the "Machine Configuration" as per the previous instance had.</br> <img src="/resources/google/compute/vm-instances-with-no-access/step8.png"/>
9. Scroll down the "Create an Instance" page, click on the "Access Scopes" option under the "Identity and API access" and choose "Allow default access" option.</br> <img src="/resources/google/compute/vm-instances-with-no-access/step9.png"/>
10. Click on the "Create" button at the bottom to make the changes.</br> <img src="/resources/google/compute/vm-instances-with-no-access/step10.png"/>
11. Once the new similar instance is up and running, delete the instance with "full access to all Cloud APIs" enabled.</br> 
12. Repeat steps number 6 - 11 to ensure Allow full access to all Cloud APIs is not selected if selecting the default service account.</br>
