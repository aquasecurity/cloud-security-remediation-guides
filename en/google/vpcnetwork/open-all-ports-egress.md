[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / VPC Network / Open All Ports Egress

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open All Ports Egress |
| **Cloud** | GOOGLE |
| **Category** | VPC Network |
| **Description** | Ensure no firewall rules allow egress to all ports and protocols |
| **More Info** | Allowing outbound traffic to all protocols and ports can lead to internal resources accessing unwanted and untrusted resources. It is a best practice to follow the principle of least privilege, and grant access to only required protocols and ports. |
| **GOOGLE Link** | https://cloud.google.com/vpc-service-controls/docs/ingress-egress-rules |
| **Recommended Action** | Restrict outbound traffic to only required protocols and ports. |

## Detailed Remediation Steps

1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Networking" to select the "Firewall rules" option under the "VPC network."</br> <img src="/resources/google/vpcnetwork/open-all-ports-egress/step2.png"/>
3. On the "Firewall rules" page, select the "Firewall rule" which needs to be verified if it allows egress to all port and protocols. </br> <img src="/resources/google/vpcnetwork/open-all-ports-egress/step3.png"/>
4. On the selected "Firewall rules", if all ports are open to the public then the selected "Firewall rule" is not as per the best standards. </br> <img src="/resources/google/vpcnetwork/open-all-ports-egress/step4.png"/>
5. Repeat steps number 2 - 4 to verify another "Firewall rule" in the network.</br>
6. Navigate to "VPC network" and choose the "Firewall rules" option under the "Networking" and select the "Firewall rule" which needs to restrict outbound traffic to known IP addresses.</br> <img src="/resources/google/vpcnetwork/open-all-ports-egress/step3.png"/>
7. On the "Firewall rules" page, click on the "Edit" button at the top and enter the "Destination IP ranges" and select the "Specified protocols and ports" as per the requirements then click on the "Save" button at the bottom to make the changes</br> <img src="/resources/google/vpcnetwork/open-all-ports-egress/step7.png"/>
8. Repeat steps number 6 - 8 to restrict ports to known IP addresses.</br> 
