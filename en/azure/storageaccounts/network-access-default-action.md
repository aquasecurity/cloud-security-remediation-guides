[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Network Access Default Action

## Quick Info

| | |
|-|-|
| **Plugin Title** | Network Access Default Action |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures that Storage Account access is restricted to trusted networks |
| **More Info** | Storage Accounts should be configured to accept traffic only from trusted networks. By default, all networks are selected but can be changed when creating a new storage account or in the firewall settings. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/common/storage-network-security |
| **Recommended Action** | Configure the firewall of each Storage Account to allow access only from known virtual networks. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Storage account. </br> <img src="/resources/azure/storageaccounts/network-access-default-action/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/storageaccounts/network-access-default-action/step3.png"/>
4. Scroll down the selected "Storage account" navigation panel and in "Settings" click on the "Firewalls and virtual networks."</br> <img src="/resources/azure/storageaccounts/network-access-default-action/step4.png"/>
5. On the "Firewalls and virtual networks" tab cross-check whether the "Allow access from" from "All networks" is selected or not. If "All networks" is selected then the selected "Storage account" access is not restricted to trusted networks. </br> <img src="/resources/azure/storageaccounts/network-access-default-action/step5.png"/>
6. Repeat steps number 2 - 5 to check other "Storage account" in the account. </br>
7. Navigate to the "Storage accounts", select the "Storage account" and click on the "Name", select the "Firewalls and virtual networks" under "Settings" that needs to disable  the "Allow access for all networks."</br> <img src="/resources/azure/storageaccounts/network-access-default-action/step7.png"/>
8. On the "Firewalls and virtual networks" tab under "Allow access from" choose the option of "Selected Network" and choose the trusted "Network" and click on the "Save" button at the top to make the changes. </br> <img src="/resources/azure/storageaccounts/network-access-default-action/step8.png"/>
9. Repeat steps number 7 - 8 to ensure that "Storage account" access is restricted to trusted networks.</br>
