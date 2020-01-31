[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / IP Forwarding Disabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | IP Forwarding Disabled |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensures that IP forwarding is disabled on all instances |
| **More Info** | Disabling IP forwarding ensures that the instance only sends and receives packets with matching destination or source IPs. |
| **GOOGLE Link** | https://cloud.google.com/vpc/docs/using-routes |
| **Recommended Action** | IP forwarding settings can only be chosen when creating a new instance. Delete the affected instances and redeploy with IP forwarding disabled. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Compute Engine" to select the "VM Instances" option. </br> <img src="/resources/google/compute/ip-forwarding-disabled/step2.png"/>
3. On the "VM Instances" page, select the VM instance which needs to be verified. </br> <img src="/resources/google/compute/ip-forwarding-disabled/step3.png"/>
4. On the "VM instance details" page, scroll down and check "IP forwarding" under the "Network Interfaces" is enabled or not for VM instances.</br> <img src="/resources/google/compute/ip-forwarding-disabled/step4.png"/>
5. Repeat steps number 2 - 4 to verify other VM instances in the network.</br>
6. Navigate to "Compute Engine", choose the "VM instances" and select the "VM instance" which needs to disabled "IP forwarding" for VM instance.</br> <img src="/resources/google/compute/ip-forwarding-disabled/step6.png"/>
7. 
