[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / VPC Network / Open Custom Ports

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open Custom Ports |
| **Cloud** | GOOGLE |
| **Category** | VPC Network |
| **Description** | Ensure that defined custom ports are not open to public. |
| **More Info** | Security groups should restrict access to ports from known networks. |
| **GOOGLE Link** | https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html |
| **Recommended Action** | Modify the security group to ensure the defined custom ports are not exposed publicly. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Networking" to select the "Firewall rules" option under the "VPC network."
3. On the "Firewall rules" page, select the "Firewall rule" which needs to be verified.
4. On the selected "Firewall rules", if custom ports are open to the public then the selected "Firewall rule" is not as per the best standards. 
5. Repeat steps number 2 - 4 to verify another "Firewall rule" in the network.
6. Navigate to "VPC network" and choose the "Firewall rules" option under the "Networking" and select the "Firewall rule" which needs to be restricted to known IP addresses.
7. On the "Firewall rules" page, click on the "Edit" button at the top and enter the "Source IP ranges" and select the "Specified protocols and ports" as per the requirements.
8. Click on the "Save" button at the bottom to make the changes.
9. Repeat steps number 6 - 8 to restrict ports to known IP addresses.
