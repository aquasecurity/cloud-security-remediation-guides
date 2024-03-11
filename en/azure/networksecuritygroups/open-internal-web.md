[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Network Security Groups / Open Internal Web

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open Internal Web |
| **Cloud** | AZURE |
| **Category** | Network Security Groups |
| **Description** | Determine if TCP port 8080 for internal web is open to the public |
| **More Info** | Internal web port 8080 is used for web applications and proxy services. Allowing Inbound traffic from any IP address to TCP port 8080 is vulnerable to exploits like backdoor trojan attacks. It is a best practice to block port 8080 from the public internet. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-network/manage-network-security-group |
| **Recommended Action** | Restrict TCP port 8080 to known IP addresses. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Click on the search bar at the top and search for Network security groups. </br> <img src="/resources/azure/networksecuritygroups/open-internal-web/step2.png"/>
3. Select the "Network security group" that needs to be verified. </br> <img src="/resources/azure/networksecuritygroups/open-internal-web/step3.png"/>
4. Click on the "Name" of the selected "Network security group" to access the port configurations. </br> <img src="/resources/azure/networksecuritygroups/open-internal-web/step4.png"/>
5. In the "Overview" tab scroll down the page and check the "Inbound security rules" under the "Settings". </br> <img src="/resources/azure/networksecuritygroups/open-internal-web/step5.png"/>
6. If the port 8080 with the protocol "TCP" is showing as "Allow" under "Actions" column for all "Source" and "Destination" then the selected "Network security group" has TCP port 8080 for Internal Web open to the public. </br> <img src="/resources/azure/networksecuritygroups/open-internal-web/step6.png"/>
7. Repeat steps number 2 - 6 to verify other "Network security groups". </br>
8. Navigate to the "Network security group" and select the security group that needs to be modified for restricting the "TCP" port for "Internal Web" on port 8080 to specific IP Address.</br> <img src="/resources/azure/networksecuritygroups/open-internal-web/step8.png"/>
9. Scroll down the left navigation panel and choose "Inbound security rules" under "Settings".</br> <img src="/resources/azure/networksecuritygroups/open-internal-web/step9.png"/>
10. Click on the Rule with PORT 8080 and "TCP" protocol in the "Name" column and in the right pane under "Source" select the "IP Address" from the dropdown menu and enter the "Source IP addresses/CIDR ranges" as per the requirement, select the required Protocol and Action and click on the "Save" option at the top of the pane. </br> <img src="/resources/azure/networksecuritygroups/open-internal-web/step10.png"/>
11. Repeat steps number 8 - 10 to restrict TCP port 8080 for Internal Web to known IP addresses.</br>
