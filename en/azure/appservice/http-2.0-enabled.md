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

1. Log in to the Microsoft Azure Management Console.
2. Find the search bar at the top and search for App Services. </br> <img src="/resources/azure/appservice/http-2.0-enabled/step2.png"/>
3. Select the "App Service" by clicking on "Name" to go to its configuration.</br> <img src="/resources/azure/appservice/http-2.0-enabled/step3.png"/>
4. Scroll down the selected "App Services" left navigation panel and under "Settings" click on the "Configuration" option.</br> <img src="/resources/azure/appservice/http-2.0-enabled/step4.png"/>
5. On the "Configuration" page select the "General settings" tab, scroll down and under the "HTTP version" check the value. It’s recommended to use version 2.0 to improve performance.</br> <img src="/resources/azure/appservice/http-2.0-enabled/step5.png"/>
6. If the "HTTP version" is not set to the latest version 2.0 then select version 2.0 from the dropdown.</br> <img src="/resources/azure/appservice/http-2.0-enabled/step6.png"/>
7. Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/appservice/http-2.0-enabled/step7.png"/>
8. Click "Continue" in the confirmation pop up to save the changes.</br> <img src="/resources/azure/appservice/http-2.0-enabled/step8.png"/>
9. Repeat steps number 3 - 8 to verify all other "Apps" are using latest Stack version in the account.</br>
