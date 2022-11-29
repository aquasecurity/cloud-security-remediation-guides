[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / Accelerated Networking Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Accelerated Networking Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** |Ensures that accelerated networking is enabled on Azure virtual machines(VM).|
| **More Info** | Accelerated networking enables single root I/O virtualization (SR-IOV) to a VM, greatly improving its networking performance. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-network/create-vm-accelerated-networking-powershell |
| **Recommended Action** | Enable accelerated networking in virtual machine network interfaces. |

## Detailed Remediation Steps

{Listed Remediation Steps}
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Virtual Machines".
3. Select the appropriate Virtual Machine by clicking on the "Name" link.
4. In the Settings section on the left menu, select "Networking"
5. Select the Network Interface by clicking on the "Name" link 
6. In Network Interface Oververview, select "Enabled Accelerated Networking" to enable accelerated networking.
7. Repeat steps 3-6 for all other Virtual Machines.
