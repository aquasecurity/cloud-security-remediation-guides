[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Storage Accounts HTTPS

## Quick Info

| | |
|-|-|
| **Plugin Title** | Storage Accounts HTTPS |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures HTTPS-only traffic is allowed to storage account endpoints |
| **More Info** | Storage Accounts can contain sensitive information and should only be accessed over HTTPS. Enabling the HTTPS-only flag ensures that Azure does not allow HTTP traffic to Storage Accounts. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/governance/policy/samples/ensure-https-storage-account |
| **Recommended Action** | Enable the HTTPS-only option for all Storage Accounts. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Storage account. </br> <img src="/resources/azure/storageaccounts/storage-accounts-https/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/storageaccounts/storage-accounts-https/step3.png"/>
4. Scroll down the selected "Storage account" navigation panel and in "Settings" click on the "Configurations".</br> <img src="/resources/azure/storageaccounts/storage-accounts-https/step4.png"/>
5. On the "Configurations" page, scroll down and check whether "Secure transfer required" is set to Disabled or Enabled. If it's set to "Disabled", then the HTTPS-only traffic is not allowed to storage account endpoints.</br> <img src="/resources/azure/storageaccounts/storage-accounts-https/step5.png"/>
6. Repeat steps 2 - 5 to check other Storage accounts.</br>
7. Navigate to the "Storage accounts", select the "Storage account" and click on the "Name", select the "Configurations" under "Settings" that needs to enable the "HTTPS".</br> <img src="/resources/azure/storageaccounts/storage-accounts-https/step7.png"/>
8. On the "Configurations" page, click on the radio button next to the Enabled under the "Secure transfer required".</br> <img src="/resources/azure/storageaccounts/storage-accounts-https/step8.png"/>
9. Click on the "Save" option at the top to make the changes.</br> <img src="/resources/azure/storageaccounts/storage-accounts-https/step9.png"/>
10. Repeat steps number 7 - 9 to enable the HTTPS-only option for all Storage Accounts.

