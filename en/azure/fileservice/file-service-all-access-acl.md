[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / File Service / File Service All Access ACL

## Quick Info

| | |
|-|-|
| **Plugin Title** | File Service All Access ACL |
| **Cloud** | AZURE |
| **Category** | File Service |
| **Description** | Ensures Storage containers do not allow full write, delete, or read ACL permissions |
| **More Info** | Storage containers can be configured to allow to read, write, or delete permissions from a share. This option should not be configured unless there is a strong business requirement. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/files/storage-how-to-create-file-share#create-a-file-share-through-the-azure-portal |
| **Recommended Action** | Disable global read, write, and delete policies on all storage containers and ensure the share ACL is configured with least privileges. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Find the search bar at the top and search for Storage. </br> <img src="/resources/azure/fileservice/file-service-all-access-acl/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration page. </br> <img src="/resources/azure/fileservice/file-service-all-access-acl/step3.png"/>
4. Scroll down and select "Containers" under "Data storage".</br> <img src="/resources/azure/fileservice/file-service-all-access-acl/step4.png"/>
5. Select a container by Right clicking and select "Access Policy" from the context menu. </br> <img src="/resources/azure/fileservice/file-service-all-access-acl/step5.png"/>
6. In the "Access Policy" pane, check the "Permissions" assosciated with the container. If the "Permissions" are "racwdl" then the policy allows full read, add, create, write, delete and list permissions and is not as per the recommended configurations.</br> <img src="/resources/azure/fileservice/file-service-all-access-acl/step6.png"/>
7. If the container has full access policy then click on the "..." link and select the "Edit" option to make the changes.</br> <img src="/resources/azure/fileservice/file-service-all-access-acl/step7.png"/>
8. In the "Edit policy" popup, open the "Permissions" dropdown.</br> <img src="/resources/azure/fileservice/file-service-all-access-acl/step8.png"/>
9. Uncheck the all the permissions and only leave the desired permissions checked and click on the "OK" button to make the changes.</br> <img src="/resources/azure/fileservice/file-service-all-access-acl/step9.png"/>
10. Click "Save" at the top of the pane to save the changes. </br> <img src="/resources/azure/fileservice/file-service-all-access-acl/step10.png"/>
11. Wait for confirmation message on the top right.</br> <img src="/resources/azure/fileservice/file-service-all-access-acl/step11.png"/>
12. Repeat steps 4 - 11 for all containers so they do not allow full write, delete, or read ACL permissions.</br>
