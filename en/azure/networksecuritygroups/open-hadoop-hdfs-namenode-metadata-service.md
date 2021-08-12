[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Network Security Groups / Open Hadoop HDFS NameNode Metadata Service

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open Hadoop HDFS NameNode Metadata Service |
| **Cloud** | AZURE |
| **Category** | Network Security Groups |
| **Description** | Determine if TCP port 8020 for HDFS NameNode metadata service is open to the public. |
| **More Info** | While some ports such as HTTP and HTTPS are required to be open to the public to function properly, more sensitive services such as Hadoop/HDFS should be restricted to known IP addresses. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-network/manage-network-security-group |
| **Recommended Action** | Restrict TCP port 8020 to known IP addresses for Hadoop/HDFS. |

## Detailed Remediation Steps


1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Network security groups. </br> <img src="/resources/azure/networksecuritygroups/open-hadoop-hdfs-namenode-metadata-service/step2.png"/>
3. Select the "Network security group" that needs to be verified. </br> <img src="/resources/azure/networksecuritygroups/open-hadoop-hdfs-namenode-metadata-service/step3.png"/>
4. Click on the "Name" of the selected "Network security group" to access the port configurations. </br> <img src="/resources/azure/networksecuritygroups/open-hadoop-hdfs-namenode-metadata-service/step4.png"/>
5. In the "Overview" tab scroll down the page and check the "Inbound security rules" under the "Settings". </br> <img src="/resources/azure/networksecuritygroups/open-hadoop-hdfs-namenode-metadata-service/step5.png"/>
6. If the "Hadoop/HDFS" for port 8020 with the protocol "TCP" is showing as "Allow" for all "Source" and "Destination" then the selected  "Network security group" has TCP port 8020 for Hadoop/HDFS is open to the public. </br> <img src="/resources/azure/networksecuritygroups/open-hadoop-hdfs-namenode-metadata-service/step6.png"/>
7. Repeat steps number 2 - 6 to verify other "Network security group." </br>
8. Navigate to the "Network security group" and select the security group that needs to modify for restricting the "TCP" port for "Hadoop/HDFS" on port 8020 to specific IP Address.</br> <img src="/resources/azure/networksecuritygroups/open-hadoop-hdfs-namenode-metadata-service/step8.png"/>
9. Scroll down the left navigation panel and choose "Inbound security rules" under "Settings."</br> <img src="/resources/azure/networksecuritygroups/open-hadoop-hdfs-namenode-metadata-service/step9.png"/>
10.  Click on the "Hadoop" protocol in the "Name" column and under "Source" select the "IP Address" from the dropdown menu and enter the "Source IP addresses/CIDR ranges" as per the requirement, select the required Protocol and Action and click on the "Save" option at the top panel. </br> <img src="/resources/azure/networksecuritygroups/open-hadoop-hdfs-namenode-metadata-service/step10.png"/>
11. Repeat steps number 8 - 10 to restrict TCP port 8020 for Hadoop/HDFS to known IP addresses.</br>
