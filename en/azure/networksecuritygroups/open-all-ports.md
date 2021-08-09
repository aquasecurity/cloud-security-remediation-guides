[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Network Security Groups / Open All Ports

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open All Ports |
| **Cloud** | AZURE |
| **Category** | Network Security Groups |
| **Description** | Ensures Network Security Groups do not expose all ports to the public |
| **More Info** | While some ports such as HTTP and HTTPS are required to be open to the public to function properly, almost all services should be restricted to known IP addresses. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-network/manage-network-security-group |
| **Recommended Action** | Restrict ports to known IP addresses |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Network security groups. </br> <img src="/resources/azure/networksecuritygroups/open-all-ports/step2.png"/>
3. Select the "Network security group" that needs to be verified. </br> <img src="/resources/azure/networksecuritygroups/open-all-ports/step3.png"/>
4. Click on the "Name" of the selected "Network security group" to access the port configurations. </br> <img src="/resources/azure/networksecuritygroups/open-all-ports/step4.png"/>
5. In the "Overview" tab scroll down the page and check the "Inbound security rules." </br> <img src="/resources/azure/networksecuritygroups/open-all-ports/step5.png"/>
6. On the "Inbound security rules" page under the "Settings", please verify all the ports apart from HTTP/HTTPS are not open to public and if any port such as SSH is open to the public then it's not as per the recommendation of Azure best practices.</br> <img src="/resources/azure/networksecuritygroups/open-all-ports/step6.png"/>
7. Repeat steps number 2 - 6 to verify other "Network security group." </br>
8. Navigate to the "Network security group" and select the security group that needs to modify for restricting the other ports to specific IP Address.</br> <img src="/resources/azure/networksecuritygroups/open-all-ports/step8.png"/>
9. Scroll down the left navigation panel and choose "Inbound security rules" under "Settings."</br> <img src="/resources/azure/networksecuritygroups/open-all-ports/step9.png"/>
10. Click on the "SSH or any" protocol in the "Name" column and under "Source" select the "IP Address" from the dropdown menu and enter the "Source IP addresses/CIDR ranges" as per the requirement, select the required Protocol and Action, enter the priority and click on the "Save" option at the top panel. </br> <img src="/resources/azure/networksecuritygroups/open-all-ports/step10.png"/>
11. Repeat steps number 8 - 10 to restrict ports to known IP addresses .</br>
