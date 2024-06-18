[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / VM Active Directory (AD) Authentication Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Active Directory (AD) Authentication Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that Azure Active Directory (AD) authentication is enabled for virtual machines. |
| **More Info** | Organizations can now improve the security of virtual machines (VMs) in Azure by integrating with Azure Active Directory (AD) authentication. Enabling Azure Active Directory (AD) authentication for Azure virtual machines (VMs) ensures access to VMs from one central point and simplifies access permission management. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/active-directory/devices/howto-vm-sign-in-azure-ad-windows |
| **Recommended Action** | Enable Azure Active Directory (AD) authentication for Azure virtual machines. |

## Detailed Remediation Steps

1. Note that this service is only available in specific Azure Regions and for specific Windows Distributions. For an up to date list, please visit https://docs.microsoft.com/en-us/azure/active-directory/devices/howto-vm-sign-in-azure-ad-windows
2. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Virtual Machines.
3. There are two ways to enable Azure AD login for a Windows VM in Azure. The first is through the Azure portal when creating a Windows VM, the second is through the use of Azure Cloud Shell when creating a Windows VM or for an existing Windows VM. 
4. Please visit https://docs.microsoft.com/en-us/azure/active-directory/devices/howto-vm-sign-in-azure-ad-windows for step by step instructions on how to make the applicable changes based on your environment configuration.