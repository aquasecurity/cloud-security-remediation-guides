[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / Disk Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | Disk Has Tags |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that Azure virtual machine disks have tags. |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/tag-resources |
| **Recommended Action** | Modify Disk and add tags. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for disks. </br> <img src="/resources/azure/virtualmachines/disk-has-tags/step2.png"/>
3. In the Disks, select a disk by clicking on the “Name” link to access the configuration changes.</br> <img src="/resources/azure/virtualmachines/disk-has-tags/step3.png"/>
4.  On the selected "Disk" page, select "Tags" the left navigation panel.</br> <img src="/resources/azure/virtualmachines/disk-has-tags/step4.png"/>
5. On the tags page enter the Name and value for the tag you want to add and click "Apply" button on the bottom of the page. </br> <img src="/resources/azure/virtualmachines/disk-has-tags/step5.png"/>

