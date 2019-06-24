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

