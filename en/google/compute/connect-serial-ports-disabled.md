[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Connect Serial Ports Disabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Connect Serial Ports Disabled |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensures connecting to serial ports is not enabled for VM instances |
| **More Info** | The serial console does not allow restricting IP Addresses, which allows any IP address to connect to instance and should therefore be disabled. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/instances/interacting-with-serial-console |
| **Recommended Action** | Ensure the Enable Connecting to Serial Ports option is disabled for all compute instances. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Compute Engine" to select the "VM Instances" option. </br> <img src="/resources/google/compute/connect-serial-ports-disabled/step2.png"/>
3. On the "VM Instances" page, select the VM instance which needs to be verified. </br> <img src="/resources/google/compute/connect-serial-ports-disabled/step3.png"/>
4. On the "VM instance details" page, scroll down and check "Enable connecting to serial ports" is enabled or not for VM instances.</br> <img src="/resources/google/compute/connect-serial-ports-disabled/step4.png"/>
5. Repeat steps number 2 - 4 to verify other VM instances in the network.</br>
6. Navigate to "Compute Engine", choose the "VM instances" and select the "VM instance" which needs to disabled "Connecting to serial ports" for VM instances.</br> <img src="/resources/google/compute/connect-serial-ports-disabled/step6.png"/>
7. On the "VM instance details" page, select the "Edit" button at the top.</br> <img src="/resources/google/compute/connect-serial-ports-disabled/step7.png"/>
8. On the "VM instance details - Edit page", unselect the checkbox next to "Enable connecting to serial ports."</br> <img src="/resources/google/compute/connect-serial-ports-disabled/step8.png"/>
9. Click on the "Save" button to make the changes.</br> <img src="/resources/google/compute/connect-serial-ports-disabled/step9.png"/>
10. Repeat steps number 6 - 9 to ensure the "Enable Connecting to Serial Ports" option is disabled for all compute instances.</br>
