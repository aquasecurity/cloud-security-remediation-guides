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

