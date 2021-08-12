[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Network Security Groups / Open SSH

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open SSH |
| **Cloud** | AZURE |
| **Category** | Network Security Groups |
| **Description** | Determine if TCP port 22 for SSH is open to the public |
| **More Info** | In order to deny ssh access to your virtual machines, you have to set your inbound security rules of Network Security Group to exclude ssh access to your Virtual Machine |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-network/manage-network-security-group |
| **Recommended Action** | Restrict TCP port 22 to known IP addresses |

## Detailed Remediation Steps


1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Network security groups. </br> <img src="/resources/azure/networksecuritygroups/open-ssh/step2.png"/>
3. Select the "Network security group" that needs to be verified. </br> <img src="/resources/azure/networksecuritygroups/open-ssh/step3.png"/>
4. Click on the "Name" of the selected "Network security group" to access the port configurations. </br> <img src="/resources/azure/networksecuritygroups/open-ssh/step4.png"/>
5. In the "Overview" tab scroll down the page and check the "Inbound security rules" under the "Settings". </br> <img src="/resources/azure/networksecuritygroups/open-ssh/step5.png"/>
6. If the "SSH" for port 22 with the protocol "TCP" is showing as "Allow" for all "Source" and "Destination" then the selected  "Network security group" has TCP port 22 for SSH open to the public. </br> <img src="/resources/azure/networksecuritygroups/open-ssh/step6.png"/>
7. Repeat steps number 2 - 6 to verify other "Network security group." </br>
8. Navigate to the "Network security group" and select the security group that needs to modify for restricting the "TCP" port for "SSH" on port 22 to specific IP Address.</br> <img src="/resources/azure/networksecuritygroups/open-ssh/step8.png"/>
9. Scroll down the left navigation panel and choose "Inbound security rules" under "Settings."</br> <img src="/resources/azure/networksecuritygroups/open-ssh/step9.png"/>
10. Click on the "SSH" protocol in the "Name" column and under "Source" select the "IP Address" from the dropdown menu and enter the "Source IP addresses/CIDR ranges" as per the requirement, select the required Protocol and Action and click on the "Save" option at the top panel. </br> <img src="/resources/azure/networksecuritygroups/open-ssh/step10.png"/>
11. Repeat steps number 8 - 10 to restrict TCP port 22 for SSH to known IP addresses.</br>
