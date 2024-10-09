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

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for App Services. </br> <img src="/resources/azure/appservice/tls-version-check/step2.png"/>
3. Select the "App Services" by clicking on the "Name" link to access the configuration changes. 
4. Scroll down to the selected "App Services" navigation panel and in "Settings", click on "Configuration".
5. Under the Platform settings tab,scroll down and check the "Minimum TLS Vesrion". It's recommended to use only latest version of the "TLS/SSL" always.</br> <img src="/resources/azure/appservice/tls-version-check/step3.png"/>    
6. Repeat steps number 2 - 5 to verify other "Apps" using latest TLS/SSL version in the account. 
