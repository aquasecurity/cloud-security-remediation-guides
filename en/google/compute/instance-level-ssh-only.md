[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Instance Level SSH Only

## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance Level SSH Only |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensures that instances are not configured to allow project-wide SSH keys |
| **More Info** | To support the principle of least privilege and prevent potential privilege escalation it is recommended that instances are not give access to project-wide SSH keys through instance metadata. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/instances/adding-removing-ssh-keys |
| **Recommended Action** | Ensure project-wide SSH keys are blocked for all instances. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Compute Engine" to select the "VM Instances" option. </br> <img src="/resources/google/compute/instance-level-ssh-only/step2.png"/>
3. On the "VM Instances" page, select the VM instance which needs to be verified. </br> <img src="/resources/google/compute/instance-level-ssh-only/step3.png"/>
4. On the "VM instance details" page, scroll down and check "Block project-wide SSH keys" is enabled or not for VM instances.</br> <img src="/resources/google/compute/instance-level-ssh-only/step4.png"/>
5. Repeat steps number 2 - 4 to verify other VM instances in the network.</br>
6. Navigate to "Compute Engine", choose the "VM instances" and select the "VM instance" which needs to enable "Block project-wide SSH keys" for VM instances.</br> <img src="/resources/google/compute/instance-level-ssh-only/step6.png"/>
7. On the "VM instance details" page, select the "Edit" button at the top.</br> <img src="/resources/google/compute/instance-level-ssh-only/step7.png"/>
8. On the "VM instance details - Edit page", select the checkbox next to "Block project-wide SSH keys."</br> <img src="/resources/google/compute/instance-level-ssh-only/step8.png"/>
9. Click on the "Save" button to make the changes.</br> <img src="/resources/google/compute/instance-level-ssh-only/step9.png"/>
10. Repeat steps number 6 - 9 to ensure project-wide SSH keys are blocked for all instances.</br>


