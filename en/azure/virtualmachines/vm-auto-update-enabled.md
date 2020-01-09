[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / VM Auto Update Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Auto Update Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that VM Auto Update is enabled for virtual machines |
| **More Info** | Enabling Auto Update on Azure virtual machines reduces the security risk of missing security patches. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-machines/windows-or-linux/maintenance-and-updates |
| **Recommended Action** | Enable VM auto update on all virtual machines |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Virtual Machines. </br> <img src="/resources/azure/virtualmachines/vm-auto-update-enabled/step2.png"/>
3. Select the "Virtual machine" by clicking the "Name" as a link to get into the configuration chanegs. </br> <img src="/resources/azure/virtualmachines/vm-auto-update-enabled/step3.png"/>
4. Scroll down the "Virtual machine" navigation panel and choose "Update management" under the "Operations" tab. </br> <img src="/resources/azure/virtualmachines/vm-auto-update-enabled/step4.png"/>
5. On the "Update management" page scrolls down and check whether the "VM Auto Update" is enabled for single Virtual machine or all Virtual Machines. If "VM Auto Update" is enabled for single VM then it will increase security risk of missing security patches for remaining VMs. </br> <img src="/resources/azure/virtualmachines/vm-auto-update-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify "VM Auto Update" for other Azure accounts. </br>
7. Navigate to "Virtual Machine", select the "Virtaul Machine" by clicking on the "Name" as a link and select the "Update management" under the "Operations" tab. </br> <img src="/resources/azure/virtualmachines/vm-auto-update-enabled/step7.png"/>
8. On the "Update Management" page select the "Enable for VMs in this subscription" and click on the "Click to select machines to enable" to choose the VMs in the subscription. </br> <img src="/resources/azure/virtualmachines/vm-auto-update-enabled/step8.png"/>
9. Once the VMs are selected click on the "Enable" button at the bottom of the page to "Enable Update Management". </br> <img src="/resources/azure/virtualmachines/vm-auto-update-enabled/step9.png"/>
10. Repeat steps number 6 - 8 to enable VMs auto update on all virtual machines. </br>
