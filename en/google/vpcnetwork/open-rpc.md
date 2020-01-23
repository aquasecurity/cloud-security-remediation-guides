[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / VPC Network / Open RPC

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open RPC |
| **Cloud** | GOOGLE |
| **Category** | VPC Network |
| **Description** | Determines if TCP port 135 for RPC is open to the public |
| **More Info** | While some ports such as HTTP and HTTPS are required to be open to the public to function properly, more sensitive services such as RPC should be restricted to known IP addresses. |
| **GOOGLE Link** | https://cloud.google.com/vpc/docs/using-firewalls |
| **Recommended Action** | Restrict TCP port 135 to known IP addresses. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Networking" to select the "Firewall rules" option under the "VPC network."</br> <img src="/resources/google/vpcnetwork/open-rpc/step2.png"/>
3. On the "Firewall rules" page, select the "Firewall rule" which needs to be verified. </br> <img src="/resources/google/vpcnetwork/open-rpc/step3.png"/>
4. On the selected "Firewall rules", if TCP port 135 for "RPC" is open to the public then the selected "Firewall rule" is not as per the best standards. </br> <img src="/resources/google/vpcnetwork/open-rpc/step4.png"/>
5. Repeat steps number 2 - 4 to verify another "Firewall rule" in the network.</br>
6. Navigate to "VPC network" and choose the "Firewall rules" option under the "Networking" and select the "Firewall rule" which needs to be restricted to known IP addresses.</br> <img src="/resources/google/vpcnetwork/open-rpc/step6.png"/>
7. On the "Firewall rules" page, click on the "Edit" button at the top and under the "Source IP ranges" enter the IP addresses as per the requirements.</br> <img src="/resources/google/vpcnetwork/open-rpc/step7.png"/>
8. Click on the "Save" button at the bottom to make the changes.</br> <img src="/resources/google/vpcnetwork/open-rpc/step8.png"/>
9. Repeat steps number 6 - 8 to restrict TCP port 135 to known IP addresses.</br> 

