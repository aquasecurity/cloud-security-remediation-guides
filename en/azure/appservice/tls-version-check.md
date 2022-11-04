[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / App Service / TLS Version Check

## Quick Info

| | |
|-|-|
| **Plugin Title** | TLS Version Check |
| **Cloud** | AZURE |
| **Category** | App Service |
| **Description** | Ensures that all web apps are using the latest version of TLS |
| **More Info** | App Services currently allows web apps to use TLS versions 1.0, 1.1 and 1.2. It is highly recommended to use the latest TLS 1.2 version for web app TLS connections. |
| **AZURE Link** | https://azure.microsoft.com/en-in/updates/app-service-and-functions-hosted-apps-can-now-update-tls-versions/ |
| **Recommended Action** | Set the minimum TLS version to 1.2 for all App Services. |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Find the search bar at the top and search for App Services. </br> <img src="/resources/azure/appservice/tls-version-check/step2.png"/>
3. Select the "App Service" by clicking on "Name" to go to its configuration.</br> <img src="/resources/azure/appservice/tls-version-check/step3.png"/>
4. Scroll down the selected "App Services" left navigation panel and under "Settings" click on the "TLS/SSL settings" option.</br> <img src="/resources/azure/appservice/tls-version-check/step4.png"/>
5. On the "TLS/SSL settings" page select the Bindings tab, scroll down and under the "Protocol Settings" check the "Minimum TLS Version". It’s recommended to use only latest version (1.2) of TLS.</br> <img src="/resources/azure/appservice/tls-version-check/step5.png"/>
6. If the "App Service" is not using the latest version of the TLS then select 1.2 from the slider.</br> <img src="/resources/azure/appservice/tls-version-check/step6.png"/>
7. Wait for the confirmation box to save changes.</br> <img src="/resources/azure/appservice/tls-version-check/step7.png"/>
8. Repeat steps number 3 - 7 to verify all other "Apps" are using latest TLS version in the account.</br>
