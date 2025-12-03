[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Network Security Groups / Open Elasticsearch

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open Elasticsearch |
| **Cloud** | AZURE |
| **Category** | Network Security Groups |
| **Description** | Determine if TCP port 9200 or 9300 for Elasticsearch is open to the public |
| **More Info** | While some ports such as HTTP and HTTPS are required to be open to the public to function properly, more sensitive services such as Elasticsearch should be restricted to known IP addresses. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-network/manage-network-security-group |
| **Recommended Action** | Restrict TCP port 9200 or 9300 to known IP addresses |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Click on the search bar at the top and search for Network security groups. </br> <img src="/resources/azure/networksecuritygroups/open-elasticsearch/step2.png"/>
3. Select the "Network security group" that needs to be verified. </br> <img src="/resources/azure/networksecuritygroups/open-elasticsearch/step3.png"/>
4. Click on the "Name" of the selected "Network security group" to access the port configurations. </br> <img src="/resources/azure/networksecuritygroups/open-elasticsearch/step4.png"/>
5. In the "Overview" tab scroll down the page and check the "Inbound security rules" under the "Settings". </br> <img src="/resources/azure/networksecuritygroups/open-elasticsearch/step5.png"/>
6. If the port 9200 or 9300 with the protocol "TCP" is showing as "Allow" under "Actions" column for all "Source" and "Destination" then the selected "Network security group" has TCP port 9200 or 9300 for Elasticsearch open to the public. </br> <img src="/resources/azure/networksecuritygroups/open-elasticsearch/step6.png"/>
7. Repeat steps number 2 - 6 to verify other "Network security groups". </br>
8. Navigate to the "Network security group" and select the security group that needs to be modified for restricting the "TCP" port for "Elasticsearch" on port 9200 or 9300 to specific IP Address.</br> <img src="/resources/azure/networksecuritygroups/open-elasticsearch/step8.png"/>
9. Scroll down the left navigation panel and choose "Inbound security rules" under "Settings".</br> <img src="/resources/azure/networksecuritygroups/open-elasticsearch/step9.png"/>
10. Click on the Rule with PORT 9200 or 9300 and "TCP" protocol in the "Name" column and in the right pane under "Source" select the "IP Address" from the dropdown menu and enter the "Source IP addresses/CIDR ranges" as per the requirement, select the required Protocol and Action and click on the "Save" option at the top of the pane. </br> <img src="/resources/azure/networksecuritygroups/open-elasticsearch/step10.png"/>
11. Repeat steps number 8 - 10 to restrict TCP port 9200 or 9300 for Elasticsearch to known IP addresses.</br>
