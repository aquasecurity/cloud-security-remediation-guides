[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Trusted MS Access Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Trusted MS Access Enabled |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures that Trusted Microsoft Services Access is enabled on Storage Accounts |
| **More Info** | Enabling firewall rules on Storage Accounts blocks all access by default. To ensure that Microsoft and Azure services that connect to the Storage Account still retain access, trusted Microsoft services should be allowed to access the storage account. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/common/storage-network-security |
| **Recommended Action** | For each Storage Account, configure an exception for trusted Microsoft services. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Storage account. </br> <img src="/resources/azure/storageaccounts/trusted-ms-access-enabled/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/storageaccounts/trusted-ms-access-enabled/step3.png"/>
4. Scroll down the selected "Storage account" navigation panel and in "Settings" click on the "Firewalls and virtual networks."</br> <img src="/resources/azure/storageaccounts/trusted-ms-access-enabled/step4.png"/>
5. On the "Firewalls and virtual networks" tab scroll down and cross-check whether the "Trusted Microsoft Services Access is enabled on Storage Accounts" or not under "Exceptions." </br> <img src="/resources/azure/storageaccounts/trusted-ms-access-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to check other "Storage account" in the account. </br>
7. Navigate to the "Storage accounts", select the "Storage account" and click on the "Name", select the "Firewalls and virtual networks" under "Settings" that needs to disable  the "Allow access for all networks."</br> <img src="/resources/azure/storageaccounts/trusted-ms-access-enabled/step7.png"/>
8. On the "Firewalls and virtual networks" tab under "Exceptions" choose the option of "Allow trusted Microsoft services to access this storage account" and click on the "Save" button at the top to make the changes. </br> <img src="/resources/azure/storageaccounts/trusted-ms-access-enabled/step8.png"/>
9. Repeat steps number 7 - 8 to ensure that each Storage Account, has an exception for trusted Microsoft services.</br>

