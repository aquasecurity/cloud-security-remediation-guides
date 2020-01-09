[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / VPC Network / Open CIFS

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open CIFS |
| **Cloud** | GOOGLE |
| **Category** | VPC Network |
| **Description** | Determines if UDP port 445 for CIFS is open to the public |
| **More Info** | While some ports such as HTTP and HTTPS are required to be open to the public to function properly, more sensitive services such as CIFS should be restricted to known IP addresses. |
| **GOOGLE Link** | https://cloud.google.com/vpc/docs/using-firewalls |
| **Recommended Action** | Restrict UDP port 445 to known IP addresses. |

## Detailed Remediation Steps

1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Networking" to select the "Firewall rules" option under the "VPC network."</br> <img src="/resources/google/vpcnetwork/open-cifs/step2.png"/>
3. On the "Firewall rules" page, select the "Firewall rule" which needs to be verified. </br> <img src="/resources/google/vpcnetwork/open-cifs/step3.png"/>
4. On the selected "Firewall rules", if "UDP port 445 for CIFS" is open to the public then the selected "Firewall rule" is not as per the best standards. </br> <img src="/resources/google/vpcnetwork/open-cifs/step4.png"/>
5. Repeat steps number 2 - 4 to verify another "Firewall rule" in the network.</br>
6. Navigate to "VPC network" and choose the "Firewall rules" option under the "Networking" and select the "Firewall rule" which needs to be restricted to known IP addresses for UDP port 445 for CIFS.</br> <img src="/resources/google/vpcnetwork/open-cifs/step6.png"/>
7. On the "Firewall rules" page, click on the "Edit" button at the top and enter the "Source IP ranges" and enter the "IP Address".</br> <img src="/resources/google/vpcnetwork/open-cifs/step7.png"/>
8. Click on the "Save" button at the bottom to make the changes.</br> <img src="/resources/google/vpcnetwork/open-cifs/step8.png"/>
9. Repeat steps number 6 - 8 to restrict UDP port 445 to known IP addresses.</br> 
