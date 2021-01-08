[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / OS Login Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | OS Login Enabled |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensures OS login is enabled for the project |
| **More Info** | Enabling OS login ensures that SSH keys used to connect to instances are mapped with IAM users. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/instances/managing-instance-access |
| **Recommended Action** | Set enable-oslogin in project-wide metadata so that it applies to all of the instances in the project. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Compute Engine" to select the "VM Instances" option. </br> <img src="/resources/google/compute/os-login-enabled/step2.png"/>
3. On the "VM Instances" page, select the VM instance which needs to be verified. </br> <img src="/resources/google/compute/os-login-enabled/step3.png"/>
4. On the "VM instance details" page, scroll down and check is there is any cutom metadata for "OS login" is enabled or not for the project.</br> <img src="/resources/google/compute/os-login-enabled/step4.png"/>
5. Repeat steps number 2 - 4 to verify other VM instances in the network.</br>
6. Navigate to "Compute Engine", choose the "VM instances" and select the "VM instance" which needs to enabled "Os login" for the project.</br> <img src="/resources/google/compute/os-login-enabled/step6.png"/>
7. On the "VM instance details" page, select the "Edit" button at the top.</br> <img src="/resources/google/compute/os-login-enabled/step7.png"/>
8. On the "VM instance details - Edit page", scroll down the page and under "Custom metadata" add the key as "enable-oslogin" and value as "TRUE."</br> <img src="/resources/google/compute/os-login-enabled/step8.png"/>
9. Click on the "Save" button to make the changes.</br> <img src="/resources/google/compute/os-login-enabled/step9.png"/>
10. Navigate to "Metadata" under the "Compute Engine" to add a project-wide metadata. Click on the "Edit" button at the top and add an entry similar to the step 8 for the key and the value and click on the "Save" button to make the changes.</br> <img src="/resources/google/compute/os-login-enabled/step10.png"/>
11. Repeat steps number 6 - 10 to set "enable-oslogin" in project-wide metadata so that it applies to all of the instances in the project.</br>
