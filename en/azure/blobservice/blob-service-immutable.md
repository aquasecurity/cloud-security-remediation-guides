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
1. Log in to the Microsoft Azure Management Console.
2. Find the search bar at the top and search for "Storage accounts". </br> <img src="/resources/azure/blobservice/blob-service-immutable/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/blobservice/blob-service-immutable/step3.png"/>
4. In the "Data Management" Section, Click on the "Data protection" tab. Enable the Soft delete for blobs or containers based on your required level and save.</br> <img src="/resources/azure/blobservice/blob-service-immutable/step4.png"/>
5. Now, in the left navigation panel click on "Containers" under "Data Storage" </br> <img src="/resources/azure/blobservice/blob-service-immutable/step5.png"/>
6. In the Containers List, select the container by clicking on the triple dots (...) on the extreme right and select "Access Policy".</br> <img src="/resources/azure/blobservice/blob-service-immutable/step6.png"/>
7. In the "Access Policy" panel, create immutable blob storage access policy in the containers (time-based or legal hold).</br> <img src="/resources/azure/blobservice/blob-service-immutable/step7.png"/>
8. To create a policy with container scope, don't check the box for Enable version-level immutability and click save.
9. Repeat steps number 5 - 8 to ensure data immutability is properly configured in blob services to protect critical data against deletion.

