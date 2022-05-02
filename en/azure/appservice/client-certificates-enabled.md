[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / App Service / Client Certificates Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Client Certificates Enabled |
| **Cloud** | AZURE |
| **Category** | App Service |
| **Description** | Ensures Client Certificates are enabled for App Services, only allowing clients with valid certificates to reach the app |
| **More Info** | Enabling Client Certificates will block all clients that do not have a valid certificate from accessing the app. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/app-service/app-service-web-configure-tls-mutual-auth#enable-client-certificates |
| **Recommended Action** | Enable incoming client certificate SSL setting for all App Services. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Find the search bar at the top and search for App Services. </br> <img src="/resources/azure/appservice/client-certificates-enabled/step2.png"/>
3. Select the "App Service" by clicking on "Name" to go to its configuration.</br> <img src="/resources/azure/appservice/client-certificates-enabled/step3.png"/>
4. Scroll down the selected "App Services" navigation panel and under "Settings" click on "Configuration" option.</br <img src="/resources/azure/appservice/client-certificates-enabled/step4.png"/>
5. On the "Configuration" page check select "General settings" tab and scroll down to "Incoming client certificates". If "Client certificate mode" is set to  "Ignore" then it will not block all clients who do not have a valid certificate from accessing the app. It is recommended to allow only requests with valid client certificates.</br> <img src="/resources/azure/appservice/client-certificates-enabled/step5.png"/>
6. If "Client certificate mode" is set to  "Ignore" then select "Require" which only allows clients with valid certificates to reach the app. Click "Save" at the top to make the change.</br> <img src="/resources/azure/appservice/client-certificates-enabled/step6.png"/>
7. Click "Continue" on the confirmation popup to complete the change.</br> <img src="/resources/azure/appservice/client-certificates-enabled/step7.png"/>
8. Repeat above steps to ensures "Client Certificates" are required for all "App Services", only allowing clients with valid certificates to reach the app. </br>
