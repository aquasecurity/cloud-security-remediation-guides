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

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Storage accounts. </br> <img src="/resources/azure/storageaccounts/log-container-public-access/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" as a link to access the configuration.</br> <img src="/resources/azure/storageaccounts/log-container-public-access/step3.png"/> 
4. On the "Storage accounts- test12diag647" page, select the "Containers" option. </br> <img src="/resources/azure/storageaccounts/log-container-public-access/step4.png"/> 
5. On the "Containers" page select the "Activity Log Container" and check the "Public Access" column. If it's not set to "Private" then the Activity Log Container have public read access.</br> <img src="/resources/azure/storageaccounts/log-container-public-access/step5.png"/> 
6. Repeat steps number 2 - 5 to verify "Activity Logs" for other Azure accounts.</br>
7. Navigate to the "Storage accounts", select the "Storage account" by clicking on the "Name", select the "Containers" option.</br>  <img src="/resources/azure/storageaccounts/log-container-public-access/step7.png"/> 
8. Select the "Actvity Log Container" which needs to set to priavte. Click on the "Change Access Level" option at the top.</br>  <img src="/resources/azure/storageaccounts/log-container-public-access/step8.png"/> 
9. On the "Change Access Level" page, click on the dropdown menu under "Public access level" and select the "Priavet (no anonymous access)" option and click on the "OK" button the make the changes.</br>  <img src="/resources/azure/storageaccounts/log-container-public-access/step9.png"/> 
10. Repeat steps number 2 - 9 to ensure the access level for the storage account containing Activity Log data is set to private.</br>

