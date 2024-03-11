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

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Virtual Machine Scale Set". </br> <img src="/resources/azure/virtualmachinescaleset/vmss-approved-extensions/step2.png"/>
3. Select the "Scale Set" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/virtualmachinescaleset/vmss-approved-extensions/step3.png"/>
4. In the left navigation panel, click on the "Extensions + applications" under "Settings".</br> <img src="/resources/azure/virtualmachinescaleset/vmss-approved-extensions/step4.png"/>
5. Select the unapproved "Extension" by clicking on by clicking on its name under Extensions tab. </br> <img src="/resources/azure/virtualmachinescaleset/vmss-approved-extensions/step5.png"/>
6. On the extension details panel click "Uninstall" button to remove the extension from scale set.</br> <img src="/resources/azure/virtualmachinescaleset/vmss-approved-extensions/step6.png"/>
7. Repeat step 5-6 to remove all the unapproved extensions from virtual machine scale set.
