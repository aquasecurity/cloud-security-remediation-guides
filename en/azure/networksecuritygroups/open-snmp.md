[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Network Security Groups / Open MySQL

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open SNMP |
| **Cloud** | AZURE |
| **Category** | Network Security Groups |
| **Description** | Determine if UDP port 161 for SNMP is open to the public |
| **More Info** | SNMP UDP 161 used by various devices and applications for logging events, monitoring and management. Allowing Inbound traffic from any external IP address on port 161 is vulnerable to DoS attack. It is a best practice to block port 161 completely unless explicitly required. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-network/manage-network-security-group |
| **Recommended Action** | Restrict UDP port 161 to known IP addresses. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Click on the search bar at the top and search for Network security groups. </br> <img src="/resources/azure/networksecuritygroups/open-mysql/step2.png"/>
3. Select the "Network security group" that needs to be verified. </br> <img src="/resources/azure/networksecuritygroups/open-mysql/step3.png"/>
4. Click on the "Name" of the selected "Network security group" to access the port configurations. </br> <img src="/resources/azure/networksecuritygroups/open-mysql/step4.png"/>
5. In the "Overview" tab scroll down the page and check the "Inbound security rules" under the "Settings". </br> <img src="/resources/azure/networksecuritygroups/open-mysql/step5.png"/>
6. If the port 161 with the protocol "UDP" is showing as "Allow" under "Actions" column for all "Source" and "Destination" then the selected "Network security group" has UDP port 161 for SNMP open to the public. </br> <img src="/resources/azure/networksecuritygroups/open-mysql/step6.png"/>
7. Repeat steps number 2 - 6 to verify other "Network security groups". </br>
8. Navigate to the "Network security group" and select the security group that needs to be modified for restricting the "UDP" port for "SNMP" on port 161 to specific IP Address.</br> <img src="/resources/azure/networksecuritygroups/open-mysql/step8.png"/>
9. Scroll down the left navigation panel and choose "Inbound security rules" under "Settings".</br> <img src="/resources/azure/networksecuritygroups/open-mysql/step9.png"/>
10. Click on the Rule with PORT 161 and "UDP" protocol in the "Name" column and in the right pane under "Source" select the "IP Address" from the dropdown menu and enter the "Source IP addresses/CIDR ranges" as per the requirement, select the required Protocol and Action and click on the "Save" option at the top of the pane. </br> <img src="/resources/azure/networksecuritygroups/open-mysql/step10.png"/>
11. Repeat steps number 8 - 10 to restrict UDP port 161 for SNMP to known IP addresses.</br>
