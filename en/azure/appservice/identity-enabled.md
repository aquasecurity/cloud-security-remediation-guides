[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / App Service / Identity Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Identity Enabled |
| **Cloud** | AZURE |
| **Category** | App Service |
| **Description** | Ensures a system or user assigned managed identity is enabled to authenticate to App Services without storing credentials in the code. |
| **More Info** | Maintaining cloud connection credentials in code is a security risk. Credentials should never appear on developer workstations and should not be checked into source control. Managed identities for Azure resources provides Azure services with a managed identity in Azure AD which can be used to authenticate to any service that supports Azure AD authentication, without having to include any credentials in code. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/app-service/overview-managed-identity |
| **Recommended Action** | Enable system or user-assigned identities for all App Services and avoid storing credentials in code. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Find the search bar at the top and search for App Services. </br> <img src="/resources/azure/appservice/identity-enabled/step2.png"/>
3. Select the "App Service" by clicking on "Name" to go to its configuration.</br> <img src="/resources/azure/appservice/identity-enabled/step3.png"/>
4. Scroll down the selected "App Services" navigation panel and in "Settings" click on the "Identity" option.</br <img src="/resources/azure/appservice/identity-enabled/step4.png"/>   
5. On the "Identity" page verify the "Status" option under "System assigned" tab. If the "Status" is set to "Off" then the "Identity" is not enabled to authenticate to App Service without storing credentials in the code. It is recommended to use Identity management to store credentials for other services such as Storage, SQL etc.</br> <img src="/resources/azure/appservice/identity-enabled/step5.png"/>   
6. If the "Status" is set to "Off" then select the "On" option next to "Status" to turn on Identity management. </br> <img src="/resources/azure/appservice/identity-enabled/step6.png"/> 
7. Click on the "Save" button at the top to ensure identity is authenticated to all services that supports Azure AD authentication, without having to include any credentials in code. </br> <img src="/resources/azure/appservice/identity-enabled/step7.png"/> 
8. Click "Yes" in the confirmation popup to complete the change.</br> <img src="/resources/azure/appservice/identity-enabled/step8.png"/> 
9. Repeat steps 3 - 8 to ensures a system or user assigned managed identity is enabled for all "App services" in the account. </br>
