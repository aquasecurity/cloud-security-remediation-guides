[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / App Service / Authentication Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Authentication Enabled |
| **Cloud** | AZURE |
| **Category** | App Service |
| **Description** | Ensures Authentication is enabled for App Services, redirecting unauthenticated users to the login page. |
| **More Info** | Enabling authentication will redirect all unauthenticated requests to the login page. It also handles authentication of users with specific providers (Azure Active Directory, Facebook, Google, Microsoft Account, and Twitter). |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/app-service/overview-authentication-authorization |
| **Recommended Action** | Enable App Service Authentication for all App Services. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for App Services. </br> <img src="/resources/azure/appservice/authentication-enabled/step2.png"/>
3. Select the "App Services" by clicking on the "Name" link to access the configuration changes.
4. Scroll down the selected "App Services" navigation panel and in "Settings" click on the "Authentication" option. </br> <img src="/resources/azure/appservice/authentication-enabled/step4.png"/>
5. Choose an Identity provider of your choice from the list of available providers. Fill in the details to set up Authentication.
6. Once set up, the Identity provider should be listed with it's App or Client ID. </br> <img src="/resources/azure/appservice/authentication-enabled/step5.png"/>