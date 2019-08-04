[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / App Service / Identity Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Identity Enabled |
| **Cloud** | AZURE |
| **Category** | App Service |
| **Description** | Ensures a system or user assigned managed identity is enabled to authenticate to App Service without storing credentials in the code. |
| **More Info** | Managing credentials in your code for authenticating to cloud services is a challenge, and maintaining the credentials secure is very important. Ideally, the credentials never appear on developer workstations and aren't checked into source control. The managed identities for Azure resources provides Azure services with an automatically managed identity in Azure AD. You can use the identity to authenticate to any service that supports Azure AD authentication, without having to include any credentials in your code. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/app-service/overview-managed-identity |
| **Recommended Action** | In your App Service go to Identity > System assigned and set it to "On" (Enabled) or go to the User assigned tab and add a user assigned managed identity. |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for App Services. </br> <img src="/resources/azure/appservice/identity-enabled/step2.png"/>
3. Select the "App Services" by clicking on the "Name" link to access the configuration changes.</br> <img src="/resources/azure/appservice/identity-enabled/step3.png"/>
4. Scroll down the selected "App Services" navigation panel and in "Settings" click on the "Identity" option.</br <img src="/resources/azure/appservice/identity-enabled/step4.png"/>   
5. On the "Identity" page verify the "Status" option under "System assigned" tab. Is the "Status" is set to "Off" then the "Identity" is not enabled to authenticate to App Service without storing credentials in the code. </br> <img src="/resources/azure/appservice/identity-enabled/step5.png"/>   
6. Repeat steps number 2 - 5 to verify other "Apps" Identity status in the account.</br>    
7. Navigate to the "App Services", select the "App Service" and click on the "Name" as a link to access the configuration, select the "Identity" under "Settings."</br> <img src="/resources/azure/appservice/identity-enabled/step7.png"/>   
8. On the "System assigned" page scroll down and select the "On" option next to "Status" and click on the "Save" button to ensure identity is authenticated to all services that supports Azure AD authentication, without having to include any credentials in code. </br> <img src="/resources/azure/appservice/identity-enabled/step8.png"/> 
9. Repeat above steps to ensures a system or user assigned managed identity is enabled to authenticate to App Service without storing credentials in the code. </br>
