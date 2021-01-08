[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Networking / Open Hadoop HDFS NameNode WebUI

## Quick Info

| | |
|-|-|
| **Plugin Title** | Open Hadoop HDFS NameNode WebUI |
| **Cloud** | ORACLE |
| **Category** | Networking |
| **Description** | Determine if TCP port 50070 and 50470 for Hadoop/HDFS NameNode WebUI service is open to the public |
| **More Info** | While some ports such as HTTP and HTTPS are required to be open to the public to function properly, more sensitive services such as Hadoop/HDFS should be restricted to known IP addresses. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Network/Concepts/securitylists.htm |
| **Recommended Action** | Restrict TCP port 50070 and 50470 to known IP addresses for Hadoop/HDFS |

## Detailed Remediation Steps
1. Log in to the Google Oracle Platform Console.
2. Scroll down the left navigation panel and choose the "Virtual Cloud Networks" under the "Networking." </br> <img src="/resources/oracle/networking/open-hadoop-hdfs-namenode-webui/step2.png"/>
3. On the "Virtual Cloud Networks" page, click on the "Name" as a link to access the "Virtual Network." </br> <img src="/resources/oracle/networking/open-hadoop-hdfs-namenode-webui/step3.png"/>
4. On the "Virtual Cloud Network Details" page, scroll down the left navigation panel and choose the "Network Security Groups" option under the "Resources." </br> <img src="/resources/oracle/networking/open-hadoop-hdfs-namenode-webui/step4.png"/>
5. On the "Network Security Groups" page, select the "Security group" by clicking on the "Name" as a link to access the security group.</br> <img src="/resources/oracle/networking/open-hadoop-hdfs-namenode-webui/step5.png"/>
6. On the "Network Security Group Details" page, under the "Security Rules" check if TCP port 50070 and 50470 for "Hadoop/HDFS NameNode WebUI" service is open to the public.Hadoop/HDFS NameNode WebUI should be restricted to known IP addresses. </br> <img src="/resources/oracle/networking/open-hadoop-hdfs-namenode-webui/step6.png"/>
7. Repeat steps number 2 - 6 to check other "Security Groups" in the account.</br>
8. Navigate to "Virtual Cloud Networks" under the "Networking", click on the "Name" as a link to access the "Virtual Network", select the "Security Group" in which TCP port 50070 and 50470 for Hadoop/HDFS NameNode WebUI needs to restrict to known IP addresses.</br> <img src="/resources/oracle/networking/open-hadoop-hdfs-namenode-webui/step8.png"/>
9. On the "Security Rules" page, click on the checkbox of the "Ingress" and click on the "Edit" button at the top to make the changes.</br> <img src="/resources/oracle/networking/open-hadoop-hdfs-namenode-webui/step9.png"/>
10. On the "Edit Rules" page, enter the "IP Address" as per requirements under the "Source CIDR" and click on the "Save" button to make the changes.</br> <img src="/resources/oracle/networking/open-hadoop-hdfs-namenode-webui/step10.png"/>
11. Repeat steps number to restrict TCP port 50070 and 50470 to known IP addresses.</br>
