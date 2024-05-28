[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Container App /Container Apps Volume Mount Configured 

## Quick Info

| | |
|-|-|
| **Plugin Title** | Container Apps Volume Mount Configured |
| **Cloud** | AZURE |
| **Category** | Container Apps |
| **Description** | Ensure that Container Apps are configured to use volume mounts. |
| **More Info** | Adding volume mounts in Azure Container Apps ensures persistent storage, enabling data integrity and seamless sharing among containers. By configuring volume mounts, data remains available even after container restarts or in case of failures, facilitating backup, scalability, and simplified management of applications. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/container-apps/storage-mounts |
| **Recommended Action** | Modify Container apps and configure volume mount. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Find the search bar at the top and search for Container apps. </br> <img src="/resources/azure/containerapps/container-apps-volume-mount/step2.png"/>
3. Select the "Conatiner App" by clicking on "Name" which needs to configure volume mounts.</br> <img src="/resources/azure/containerapps/container-apps-volume-mount/step3.png"/>
4. Scroll down the left navigation panel and choose "Volume".</br> <img src="/resources/azure/containerapps/container-apps-volume-mount/step4.png"/>
5. Click on add option to add the volume to the container app".</br> <img src="/resources/azure/containerapps/container-apps-volume-mount/step5.png"/>
6. Add the volume type  of your choice to the container app and enable the mount on volume.</br> <img src="/resources/azure/containerapps/container-apps-volume-mount/step6.png"/>
7. Click on save button to save the volume configure with mount. </br> <img src="/resources/azure/containerapp/container-apps-volume-mount/step7.png"/>
8. In case of already present unmounted volume, select on the "volume" by clicking on "Name" .</br> <img src="/resources/azure/containerapps/container-apps-volume-mount/step8.png"/>
9. Configure the mount and click on save button to save the configuration. </br> <img src="/resources/azure/containerapps/container-apps-volume-mount/step9.png"/>
10. Repeat steps number 4 - 9 to configure container apps with volume mounts.</br>