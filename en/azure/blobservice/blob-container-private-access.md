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
2. Select the "Search resources, services, and docs" option at the top and search for Storage account. </br> <img src="/resources/azure/blobservice/blob-container-private-access/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/blobservice/blob-container-private-access/step3.png"/>
4. Click on the "Overveiw" in the selected "Storage account" and scroll down the right side of the settings and click on the "Blobs" option. </br> <img src="/resources/azure/blobservice/blob-container-private-access/step4.png"/>
5. Under the "Blobs" check for the "Public Access" and if it's set to Blob/Container then the selected "Blob" have anonymous public access level.</br> <img src="/resources/azure/blobservice/blob-container-private-access/step5.png"/>
6. Repeat steps number 2 - 5 to verify other Blobs in the "Storage accounts." </br>
7. Navigate to the "Storage accounts", select the "Storage account" and click on the "Name", select the "Overview" options and select the "Blob" which needs to have "Private access".</br> <img src="/resources/azure/blobservice/blob-container-private-access/step7.png"/>
8. Select the "Blob" and click on the "Change access level" at the top panel. </br> <img src="/resources/azure/blobservice/blob-container-private-access/step8.png"/>
9. On the "Change access level" tab, select the "Private (no anonymous access)" and click on the "OK" button to make the necessary changes.</br> <img src="/resources/azure/blobservice/blob-container-private-access/step9.png"/>
10. Repeat steps number 7 - 9 to ensure that all blob containers do not have anonymous public access level.</br>
