[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Storage Accounts / Log Container Public Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Log Container Public Access |
| **Cloud** | AZURE |
| **Category** | Storage Accounts |
| **Description** | Ensures that the Activity Log Container does not have public read access |
| **More Info** | The container used to store Activity Log data should not be exposed publicly to avoid data exposure of sensitive activity logs. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/blobs/storage-manage-access-to-resources |
| **Recommended Action** | Ensure the access level for the storage account containing Activity Log data is set to private. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Storage accounts. </br> <img src="/resources/azure/storageaccounts/log-container-public-access/step2.png"/>
3. Select the "Storage account" by clicking on its "Name" to get into its configuration page.</br> <img src="/resources/azure/storageaccounts/log-container-public-access/step3.png"/> 
4. On the "Storage accounts" page, select the "Containers" under "Data storage". </br> <img src="/resources/azure/storageaccounts/log-container-public-access/step4.png"/> 
5. On the "Containers" page select the "Activity Log Container" and check the "Public Access" column. If it's not set to "Private" then the Activity Log Container has public read access.</br> <img src="/resources/azure/storageaccounts/log-container-public-access/step5.png"/> 
6. Select the "Actvity Log Container" which needs to be set to priavte. Click on the "Change access level" option at the top.</br>  <img src="/resources/azure/storageaccounts/log-container-public-access/step6.png"/> 
7. On the "Change access level" page, click on the dropdown menu under "Public access level" and select the "Private (no anonymous access)" option.</br>  <img src="/resources/azure/storageaccounts/log-container-public-access/step7.png"/> 
8. Click on the "OK" button to save the changes.</br>  <img src="/resources/azure/storageaccounts/log-container-public-access/step8.png"/> 
9. Repeat steps number 2 - 8 to ensure the access level for the storage account containing Activity Log data is set to private.</br>

