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

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Storage accounts". </br> <img src="/resources/azure/storageaccounts/network-access-default-action/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration page. </br> <img src="/resources/azure/storageaccounts/network-access-default-action/step3.png"/>
4. Scroll down the selected "Storage account" navigation panel and click on "Networking" under "Security + networking".</br> <img src="/resources/azure/storageaccounts/network-access-default-action/step4.png"/>
5. Once on the "Networking page" click on tab "Firewalls and virtual networks". </br> <img src="/resources/azure/storageaccounts/network-access-default-action/step4.png"/>
6. On the "Firewalls and virtual networks" tab check the option selected under "Public network access". If "Enabled from all networks" is selected then the selected "Storage account" access is not restricted to trusted networks. </br> <img src="/resources/azure/storageaccounts/network-access-default-action/step6.png"/>
7. To restrict the selected storage account's access to all networks, under "Public network access" select option "Enabled from selected virtual networks and IP addresses" and choose the trusted "Virtual Network".</br> <img src="/resources/azure/storageaccounts/network-access-default-action/step7.png"/>
8. Click on "Save" button at the top to make the changes.</br> <img src="/resources/azure/storageaccounts/network-access-default-action/step8.png"/>
9. Repeat steps number 3 - 8 to ensure that "Storage account" access is restricted to trusted networks.</br>
