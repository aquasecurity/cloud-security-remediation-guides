[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Network Security Groups / Deny SSH Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Deny SSH Access |
| **Cloud** | AZURE |
| **Category** | Network Security Groups |
| **Description** | Ensures that all Network Security Group Security Rules deny public SSH access |
| **More Info** | Inbound security group rules should prohibit inbound SSH access from the global address. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-restrict-access-through-internet-facing-endpoints |
| **Recommended Action** | For each Network Security Group attached to a Virtual Machine instance, ensure that the inbound SSH port is appropriately restricted. |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Network security groups. </br> <img src="/resources/azure/networksecuritygroups/deny-ssh-access/step2.png"/>
3. Select the "Network security group" that needs to be verified. </br> <img src="/resources/azure/networksecuritygroups/deny-ssh-access/step3.png"/>
4. Click on the "Name" of the selected "Network security group" to access the port configurations. </br> <img src="/resources/azure/networksecuritygroups/deny-ssh-access/step4.png"/>
5. In the "Overview" tab scroll down the page and check the "Inbound security rules." </br> <img src="/resources/azure/networksecuritygroups/deny-ssh-access/step5.png"/>
6. If the "SSH" for port 22 with the protocol "TCP" is showing as "Allow" for all "Source" and "Destination" then the selected  "Network security group" has SSH access from the global address.  </br> <img src="/resources/azure/networksecuritygroups/deny-ssh-access/step6.png"/>
7. Repeat steps number 2 - 6 to verify other "Network security group." </br>
8. Navigate to the "Network security group" and select the security group that needs to modify for restricting the "TCP" port for "SSH" on port 22 to specific IP Address.</br> <img src="/resources/azure/networksecuritygroups/deny-ssh-access/step8.png"/>
9. Scroll down the left navigation panel and choose "Inbound security rules" under "Settings."</br> <img src="/resources/azure/networksecuritygroups/deny-ssh-access/step9.png"/>
10. Click on the "SSH" protocol in the "Name" column and under "Source" select the "IP Address" from the dropdown menu and enter the "Source IP addresses/CIDR ranges" as per the requirement and click on the "Save" option at the top panel. </br> <img src="/resources/azure/networksecuritygroups/deny-ssh-access/step10.png"/>
11. Repeat steps number 8 - 10 to ensure that the inbound SSH port is appropriately restricted. </br>
