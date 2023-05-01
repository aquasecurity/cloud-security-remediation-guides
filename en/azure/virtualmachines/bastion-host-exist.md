[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / Azure Bastion Host Exists

## Quick Info

| | |
|-|-|
| **Plugin Title** | Azure Bastion Host Exists |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensure that Azure Bastion Host exists. |
| **More Info** | Bastion provides secure RDP and SSH connectivity to all of the VMs in the virtual network in which it is provisioned. Using Azure Bastion protects your virtual machines from exposing RDP/SSH ports to the outside world, while still providing secure access using RDP/SSH. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/bastion/bastion-overview |
| **Recommended Action** | Create an Azure Bastion Host in azure account. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Bastions. </br> <img src="/resources/azure/virtualmachines/bastion-host-exist/step2.png"/>
3. On Bastion Page Click on Create from navigation bar on the page. </br> <img src="/resources/azure/virtualmachines/bastion-host-exist/step3.png"/>
4. Enter the required information e.g Select subscription, region enter the host name, Instance Count, and virtual network information. For virtual network create a subnet named AzureBastionSubnet with /26.</br> <img src="/resources/azure/virtualmachines/bastion-host-exist/step4.png"/>
5. After the entering these information Click next on bottom of the page and enter all required information. In the same complete All steps and Review the entered information and Click Create.</br> <img src="/resources/azure/virtualmachines/bastion-host-exist/step5.png"/>
6. After sometime you will be able to see Bastion host up and running.
