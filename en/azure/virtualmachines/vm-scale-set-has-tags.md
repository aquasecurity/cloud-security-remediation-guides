[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / VM Scale Set Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Scale Set Has Tags |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensure that Azure virtual machine scale set have tags associated |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AZURE Link** | https://learn.microsoft.com/bs-latn-ba/azure/virtual-machines/tag-portal |
| **Recommended Action** | Modify VM scale set and add tags |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Virtual Machine Scale sets. </br> <img src="/resources/azure/virtualmachines/vm-scale-set-has-tags/step2.png"/>
3. Select the "Virtual machine Scale Sets" by clicking the "Name" as a link to get into the configuration changes. </br> <img src="/resources/azure/virtualmachines/vm-scale-set-has-tags/step3.png"/>
4. On "Virtual machine" navigation panel and choose "Tags". </br> <img src="/resources/azure/virtualmachines/vm-scale-set-has-tags/step4.png"/>
5. Enter the tags Name and value then click "Apply" button on the bottom of the page to save tags.</br> <img src="/resources/azure/virtualmachines/vm-scale-set-has-tags/step5.png"/>