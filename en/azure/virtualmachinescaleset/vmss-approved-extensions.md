[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machine Scale Set / VM Scale Set Approved Extensions

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Scale Set Approved Extensions |
| **Cloud** | AZURE |
| **Category** | Virtual Machine Scale Set |
| **Description** | Ensures that approved Virtual Machine Scale Set extensions are installed |
| **More Info** | Extensions are small applications that provide post-deployment configuration and automation on Azure VMs. Extensions installed should be approved by the organization to meet the organizational security requirements. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/virtual-machines/extensions/overview |
| **Recommended Action** | Uninstall unapproved virtual machine scale set extensions. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Virtual machine scale sets".
3. Select the corresponding scale set by clicking on the "name" link
4. Once the scale set is selected, select "Extensions + Applications".
5. Review the list of installed extensions and verify that only approved extensions are present. Uninstall any unapproved extensions if found.
6. Repeat steps 3-5 for all applicable scale set instances.
