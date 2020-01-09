[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Blob Service / Blob Service Immutable

## Quick Info

| | |
|-|-|
| **Plugin Title** | Blob Service Immutable |
| **Cloud** | AZURE |
| **Category** | Blob Service |
| **Description** | Ensures data immutability is properly configured for blob services to protect critical data against deletion |
| **More Info** | Immutable storage helps store data securely by protecting critical data against deletion. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blob-immutable-storage#Getting-started |
| **Recommended Action** | Enable a data immutability policy for all storage containers in the Azure storage account. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Storage account. </br> <img src="/resources/azure/blobservice/blob-service-immutable/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/blobservice/blob-service-immutable/step3.png"/>
4. Click on the "Overveiw" in the selected "Storage account" and scroll down the right side of the settings and click on the "Blobs" option. </br> <img src="/resources/azure/blobservice/blob-service-immutable/step4.png"/>
5. On the "Blobs" page select the "Blob" by clicking on the "Name" as a link to access the configuration changes.</br> <img src="/resources/azure/blobservice/blob-service-immutable/step5.png"/>
6. In the selected "Blob", click on the "Access Policy" and check the "Permissions" assosciated with the "Blob". If the "Blob" allow full read,add,create,write, delete, or list permissions then the selected "Blob" is not properly configured in blob services to protect critical data against deletion.</br> <img src="/resources/azure/blobservice/blob-service-immutable/step6.png"/>
7. Repeat steps number 2 - 6 to verify other "Blobs" in the Storage accounts. </br>
8. Navigate to the "Storage accounts", select the "Storage account" and click on the "Name", select the "Overview" options and select the "Blob" by clicking on the "Name" as a link to access the configurations.</br> <img src="/resources/azure/blobservice/blob-service-immutable/step8.png"/>
9. On the "Blob" configuration click on the "Access Policy" option and select the "Edit" option to make the changes.</br> <img src="/resources/azure/blobservice/blob-service-immutable/step9.png"/>
10. Uncheck the "Add/Write/Detele/List" policies under the "Permissions" and click on the "OK" button to make the changes.</br> <img src="/resources/azure/blobservice/blob-service-immutable/step10.png"/>
11. Repeat steps number 8 - 10 to ensures data immutability is properly configured in blob services to protect critical data against deletion.</br>
