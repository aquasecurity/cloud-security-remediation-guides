[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / VPC Network / Private Access Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Private Access Enabled |
| **Cloud** | GOOGLE |
| **Category** | VPC Network |
| **Description** | Ensures Private Google Access is enabled for all Subnets |
| **More Info** | Private Google Access allows VM instances on a subnet to reach Google APIs and services without an IP address. This creates a more secure network for the internal communication. |
| **GOOGLE Link** | https://cloud.google.com/vpc/docs/configure-private-google-access |
| **Recommended Action** | 1. Enter the VPC Network service. 2. Enter the VPC. 3. Select the subnet in question. 4. Edit the subnet and enable Private Google Access. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Networking" to select the "VPC networks" option under the "VPC network."</br> <img src="/resources/google/vpcnetwork/private-access-enabled/step2.png"/>
3. On the VPC network page, select the VPC which needs to be verified. </br> <img src="/resources/google/vpcnetwork/private-access-enabled/step3.png"/>
4. On the "Subnet details" page, scroll down and check the "Private Google access" option. If it's set to "Off" then the selected VPC don't have "Google Access" enabled for all the subnets.</br> <img src="/resources/google/vpcnetwork/private-access-enabled/step4.png"/>
5. Repeat steps number 2 - 4 to verifiy other VPC's in the account.</br>
6. Navigate to "VPC network" and choose the "VPC networks" option under the "Networking" and select the "VPC network" which needs to enabled "Google Access" for all the subents.</br> <img src="/resources/google/vpcnetwork/private-access-enabled/step6.png"/>
7. On the "Subnet details" page, click on the "Edit" button at the top. </br> <img src="/resources/google/vpcnetwork/private-access-enabled/step7.png"/>
8. On the "Subnet details Edit" page, scroll down the page and click on the "ON" option below the "Private Google access."</br> <img src="/resources/google/vpcnetwork/private-access-enabled/step8.png"/>
9. Click on the "Save" button at the bottom of the page to make the changes.</br> <img src="/resources/google/vpcnetwork/private-access-enabled/step9.png"/>
10. Repeat steps number 6 - 9 to ensures "Private Google Access" is enabled for all Subnets.</br>
