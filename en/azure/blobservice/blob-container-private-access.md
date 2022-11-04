[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Blob Service / Blob Container Private Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Blob Container Private Access |
| **Cloud** | AZURE |
| **Category** | Blob Service |
| **Description** | Ensures that all blob containers do not have anonymous public access set |
| **More Info** | Blob containers set with public access enables anonymous users to read blobs within a publicly accessible container without authentication. All blob containers should have private access configured. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blobs-introduction |
| **Recommended Action** | Ensure each blob container is configured to restrict anonymous access |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Find the search bar at the top and search for Storage account. </br> <img src="/resources/azure/blobservice/blob-container-private-access/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/blobservice/blob-container-private-access/step3.png"/>
4. In the left navigation panel click on "Containers" under "Data storage".</br> <img src="/resources/azure/blobservice/blob-container-private-access/step4.png"/>
5. In the Containers List, select the container for which the column "Public access level" shows "Blob" or "Container" and click on "Change access level" button at the top.</br> <img src="/resources/azure/blobservice/blob-container-private-access/step5.png"/>
6. In the "Change access level" pop up the "Public access level" dropdown should be set to "Private(no anonymous access)". If it is set to "Blob" or "Container" then anonymous requests are allowed at the service level and this is against azure best practices.<img src="/resources/azure/blobservice/blob-container-private-access/step6.png"/>
7. In the "Change access level" pop up click on the "Public access level" dropdown and select "Private(no anonymous access)" and click "OK" to make the necessary changes.<img src="/resources/azure/blobservice/blob-container-private-access/step7.png"/>
8. Repeat steps number 5 - 7 to ensure that all blob containers have private access level.</br>
