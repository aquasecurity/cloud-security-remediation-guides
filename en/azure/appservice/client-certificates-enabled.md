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
2. Select the "Search resources, services, and docs" option at the top and search for App Services. </br> <img src="/resources/azure/appservice/client-certificates-enabled/step2.png"/>
3. Select the "App Services" by clicking on the "Name" link to access the configuration changes.
4. Scroll down the selected "App Services" navigation panel and in "Settings" click on "Configuration" option. </br> <img src="/resources/azure/appservice/client-certificates-enabled/step3.png"/>
5. Under the "Incoming client certificates" section, Choose "Require" in Client certificate mode. </br> <img src="/resources/azure/appservice/client-certificates-enabled/step4.png"/>
