[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / App Service / Authentication Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Authentication Enabled |
| **Cloud** | AZURE |
| **Category** | App Service |
| **Description** | Ensures Authentication is enabled for App Services, redirecting unauthenticated users to the login page. |
| **More Info** | Enabling authentication will redirect all unauthenticated requests to the login page. It also handles authentication of users with specific providers (Azure Entra ID, Facebook, Google, Microsoft Account, and Twitter). |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/app-service/overview-authentication-authorization |
| **Recommended Action** | Enable App Service Authentication for all App Services. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Find the search bar at the top and search for App Services.</br> <img src="/resources/azure/appservice/authentication-enabled/step2.png"/>
3. Select the "App Service" by clicking on "Name" to go to its configuration.</br> <img src="/resources/azure/appservice/authentication-enabled/step3.png"/>
4. Scroll down the selected "App Services" navigation panel and under "Settings" click on "Authentication".</br> <img src="/resources/azure/appservice/authentication-enabled/step4.png"/>
5. On the "Authentication" page check if "App Service Authentication" is "Disabled". If it's "Disabled", then all unauthenticated requests to the app will not be redirected to the login page. It is recommended to have authentication enabled for all requests.</br> <img src="/resources/azure/appservice/authentication-enabled/step5.png"/>
6. If the "App Service Authentication" is "Disabled", then click on "Enable authentication" button to enable authentication.</br> <img src="/resources/azure/appservice/authentication-enabled/step5.png"/>
7. Wait for the confirmation message on top right to ensure authentication is now enabled.</br> <img src="/resources/azure/appservice/authentication-enabled/step7.png"/>
8. If there is no "Identity provider" then you will see the "Add identity provider" button. </br> <img src="/resources/azure/appservice/authentication-enabled/step8.png"/>
9. Click on the "Add identity provider" button and choose your desired "Identity provider" by selecting the relevant provider's name.</br> <img src="/resources/azure/appservice/authentication-enabled/step9.png"/>
10. Now configure the behavior and click "Add" to complete the setup.</br> <img src="/resources/azure/appservice/authentication-enabled/step10.png"/>
11. Verify that "Authentication" is now enabled.</br> <img src="/resources/azure/appservice/authentication-enabled/step11.png"/>
12. Repeat steps 3 to 11 to enable "Authentication" across all "App Services" in the account.</br>
