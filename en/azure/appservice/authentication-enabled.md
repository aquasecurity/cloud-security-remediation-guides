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
3. Select the "App Services" by clicking on the "Name" link to access the configuration changes.</br> <img src="/resources/azure/appservice/authentication-enabled/step3.png"/>
4. Scroll down the selected "App Services" navigation panel and in "Settings" click on the "Authentication / Authorization" option.</br> <img src="/resources/azure/appservice/authentication-enabled/step4.png"/>
5. On the "Authentication / Authorization" page check if "App Service Authentication" is "ON/OFF". If it's turned "OFF" all unauthenticated requests to the login page will not be redirected. </br> <img src="/resources/azure/appservice/authentication-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to cross check "Authentication / Authorization" for other "App Services."</br>
7. Navigate to the "App Services", select the "App Service" and click on the "Name", select the "Authentication / Authorization" under "Settings."</br> <img src="/resources/azure/appservice/authentication-enabled/step7.png"/>
8. Click on the "ON" option under "App Service Authentication" and click on the "Save" button at the top to make the chamges.</br> <img src="/resources/azure/appservice/authentication-enabled/step8.png"/>
9. Repeat above steps for enabling "Authentication" to redirect all unauthenticated requests to the login page.</br>
