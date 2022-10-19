[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Container Registry / ACR Admin User

## Quick Info

| | |
|-|-|
| **Plugin Title** | ACR Admin User |
| **Cloud** | AZURE |
| **Category** | Container Registry |
| **Description** | Ensures that the admin user is not enabled on container registries |
| **More Info** | Azure Container Registries have an admin user that is designed for testing. This should be disabled by default to avoid sharing confidential admin credentials. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/container-registry/container-registry-authentication |
| **Recommended Action** | Ensure that the admin user is disabled for each container registry. |

## Detailed Remediation Steps

1. Login to the Azure portal.
2. In the search bar at the top search for container registries and click on "Conatiner registries".<br/> <img src="/resources/azure/containerregistry/acr-admin-user/step2.png"/>
3. On the container registries page, click on the "Name" link to go to the configuration page.<br/> <img src="/resources/azure/containerregistry/acr-admin-user/step3.png"/>
4. On the container registry pane that opens, click on "Access keys" under "Settings" in the left navigation panel.<br/> <img src="/resources/azure/containerregistry/acr-admin-user/step4.png"/>
5. In the keys panel, if you see "Enabled" next to "Admin user" then the admin user is enabled for the container registry. This is a security risk and against the Azure recommended practices.<br/> <img src="/resources/azure/containerregistry/acr-admin-user/step5.png"/>
6. Click on the slider to "Disable" the admin user.<br/> <img src="/resources/azure/containerregistry/acr-admin-user/step6.png"/>
7. Repeat steps 3 - 6 for all other container registries.



