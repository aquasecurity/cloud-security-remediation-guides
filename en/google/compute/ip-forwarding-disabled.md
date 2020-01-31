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
7. On the "VM instance details" page, select the "CREATE SIMILAR" button at the top.</br> <img src="/resources/google/compute/ip-forwarding-disabled/step7.png"/>
8. Enter the "Name" of the instance, Region, Choose the "Machine Configuration" as per the previous instance had.</br> <img src="/resources/google/compute/ip-forwarding-disabled/step8.png"/>
9. Scroll down the "Create an Instance" page, click on the "Management, security, disks, networking, sole tenancy" option, choose "Networking" and click on the pencil icon next to the "default" under "Network Interfaces."</br> <img src="/resources/google/compute/ip-forwarding-disabled/step9.png"/>
10. On the "Network Interfaces" tab, scroll down the page and select "OFF" from the dropdown menu under the "IP Forwarding" option.</br> <img src="/resources/google/compute/ip-forwarding-disabled/step10.png"/>
11. Click on the "Create" button at the bottom to make the changes.</br> <img src="/resources/google/compute/ip-forwarding-disabled/step11.png"/>
12. Once the new similar instance is up and running, delete the instance with "IP forwarding" enabled.</br> 
13. Repeat steps number 6 - 12 so that IP forwarding settings can only be chosen when creating a new instance. Delete the affected instances and redeploy with IP forwarding disabled.</br>
