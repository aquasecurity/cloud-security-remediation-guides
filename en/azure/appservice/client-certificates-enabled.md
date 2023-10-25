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
3. Select the "App Services" by clicking on the "Name" link to access the configuration changes.</br> <img src="/resources/azure/appservice/client-certificates-enabled/step3.png"/>
4. On left navigation panel that opens, click on Configuration tab.</br <img src="/resources/azure/appservice/client-certificates-enabled/step4.png"/>
5. Select General settings tab on the Configuration page that opens. </br> <img src="/resources/azure/appservice/client-certificates-enabled/step5.png"/>
6. Scroll down to check for Incoming client certificates at the bottom and select one of the following "Required", "Allowed", or "Optional", according to requirement.
.</br> <img src="/resources/azure/appservice/client-certificates-enabled/step7.png"/>
7. Repeat above steps to ensures "Client Certificates" are enabled for "App Services", only allowing clients with valid certificates to reach the app. </br>
</br> "NOTE: This plugin shows positive result when HTTP2.0 is enabled"
