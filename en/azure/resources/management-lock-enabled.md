[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Resources / Management Lock Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Management Lock Enabled |
| **Cloud** | AZURE |
| **Category** | Resources |
| **Description** | Ensures that resources tagged as locked are actually locked |
| **More Info** | Enabling Management Locks ensures that critical resources cannot be inadvertently modified or deleted. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/azure-resource-manager/resource-group-lock-resources |
| **Recommended Action** | Ensure that critical resources such as storage, VMs etc have management lock enabled. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Storage accounts". </br> <img src="/resources/azure/resources/management-lock-enabled/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/resources/management-lock-enabled/step3.png"/>
4. In the left navigation panel, click on the "Locks" under "Settings".</br> <img src="/resources/azure/resources/management-lock-enabled/step4.png"/>
5. If you do not see any locks enabled then the resource is not protected against advertent deletion by a managament lock.</br> <img src="/resources/azure/resources/management-lock-enabled/step5.png"/>
6. To ensure that management lock is enabled, click the "Add" button at the top and select "Read only" from the dropdown "Lock type" in the "Add" pop up and click "OK". </br> <img src="/resources/azure/resources/management-lock-enabled/step6.png"/>
7. Ensure all other critical resources have management lock enabled.</br> <img src="/resources/azure/resources/management-lock-enabled/step7.png"/>
