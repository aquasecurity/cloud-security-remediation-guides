[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / App Service / HTTP 2.0 Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | HTTP 2.0 Enabled |
| **Cloud** | AZURE |
| **Category** | App Service |
| **Description** | Ensures the latest HTTP version is enabled for App Services |
| **More Info** | Enabling HTTP2.0 ensures that the App Service has the latest technology which improves server performance |
| **AZURE Link** | https://azure.microsoft.com/en-us/blog/announcing-http-2-support-in-azure-app-service/ |
| **Recommended Action** | Enable HTTP 2.0 support in the general settings for all App Services |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for App Services. </br> <img src="/resources/azure/appservice/http-2.0-enabled/step2.png"/>
3. Select the "App Services" by clicking on the "Name" link to access the configuration changes.
4. Scroll down the selected "App Services" navigation panel and in "Settings" click on the "Configuration" option.
5. On the "Configuration" page select the General settings tab,scroll down and on the HTTP version box check the version in use. If HTTP version is not set to HTTP 2.0 then the selected App service is not using the latest technology. </br> <img src="/resources/azure/appservice/http-2.0-enabled/step3.png"/>


