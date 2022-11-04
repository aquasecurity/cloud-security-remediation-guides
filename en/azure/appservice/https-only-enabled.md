[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / App Service / HTTPS Only Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | HTTPS Only Enabled |
| **Cloud** | AZURE |
| **Category** | App Service |
| **Description** | Ensures HTTPS Only is enabled for App Services, redirecting all HTTP traffic to HTTPS |
| **More Info** | Enabling HTTPS Only traffic will redirect all non-secure HTTP requests to HTTPS. HTTPS uses the SSL/TLS protocol to provide a secure connection. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/app-service/app-service-web-tutorial-custom-ssl#enforce-https |
| **Recommended Action** | Enable HTTPS Only support SSL settings for all App Services |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Find the search bar at the top and search for App Services. </br> <img src="/resources/azure/appservice/https-only-enabled/step2.png"/>
3. Select the "App Service" by clicking on "Name" to go to its configuration.</br> <img src="/resources/azure/appservice/https-only-enabled/step3.png"/>
4. Scroll down the selected "App Services" left navigation panel and under "Settings" click on the "TLS/SSL settings" option.</br> <img src="/resources/azure/appservice/https-only-enabled/step4.png"/>
5. On the "TLS/SSL settings" page select the Bindings tab, scroll down and under the "Protocol Settings" check whether "HTTPS Only" is set to "Off". It’s recommended to set HTTPS only to "On" to allow only secure traffic.</br> <img src="/resources/azure/appservice/https-only-enabled/step5.png"/>
6. If the "App Service" is not using "HTTPS only" then select "On" from the slider.</br> <img src="/resources/azure/appservice/https-only-enabled/step6.png"/>
7. Wait for the confirmation box to save changes.</br> <img src="/resources/azure/appservice/https-only-enabled/step7.png"/>
8. Repeat steps number 3 - 7 to verify all other "Apps" are using HTTPS only in the account.</br>
