[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / App Service / Client Certificates Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Client Certificates Enabled |
| **Cloud** | AZURE |
| **Category** | App Service |
| **Description** | Ensures Client Certificates are enabled for your App Service, only allowing clients with valid certificates to reach the app |
| **More Info** | Enabling Client Certificates will block all clients who do not have a valid certificate from accessing the app. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/app-service/app-service-web-configure-tls-mutual-auth#enable-client-certificates |
| **Recommended Action** | In your App Service go to SSL Settings > Incoming client certificates and set it to "On" (Enabled). |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for App Services. </br> <img src="/resources/azure/appservice/client-certificates-enabled/step2.png"/>
3. Select the "App Services" by clicking on the "Name" link to access the configuration changes.</br> <img src="/resources/azure/appservice/client-certificates-enabled/step3.png"/>
4. Scroll down the selected "App Services" navigation panel and in "Settings" click on the "TLS/SSL settings" option.</br <img src="/resources/azure/appservice/client-certificates-enabled/step4.png"/>
5. On the "TLS/SSL settings" page check if "Incoming client certificates" is "ON/OFF". If it's turned "OFF" then it will not block all clients who do not have a valid certificate from accessing the app. </br>
6. Repeat steps number 2 - 5 to verify other "Apps" SSL settings in the account.</br>
7. Navigate to the "App Services", select the "App Service" and click on the "Name" as a link to access the configuration, select the "TLS/SSL settings" under "Settings."</br>
8. On the "Protocol Settings" page click on the "ON" option next to "Incoming client certificates" which only allows clients with valid certificates to reach the app. </br>
9. Repeat above steps to ensures "Client Certificates" are enabled for "App Services", only allowing clients with valid certificates to reach the app. </br>
