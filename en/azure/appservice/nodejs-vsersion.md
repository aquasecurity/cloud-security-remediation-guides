[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / App Service / PHP Version

## Quick Info

| | |
|-|-|
| **Plugin Title** | NodeJS Version |
| **Cloud** | AZURE |
| **Category** | App Service |
| **Description** | Ensures the latest version of NodeJS is installed for all App Services |
| **More Info** | Installing the latest version of NodeJS will reduce the security risk of missing security patches. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/app-service/web-sites-nodejs-configure |
| **Recommended Action** | Select the latest version of NodeJS for all NodeJS-based App Services |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Find the search bar at the top and search for App Services. </br> <img src="/resources/azure/appservice/nodejs-version/step2.png"/>
3. Select the "App Service" by clicking on "Name" to go to its configuration.</br> <img src="/resources/azure/appservice/nodejs-version/step3.png"/>
4. Scroll down the selected "App Services" left navigation panel and in "Settings" click on the "Configuration" option.</br> <img src="/resources/azure/appservice/nodejs-version/step4.png"/>
5. On the "Configuration" page select the General settings tab, scroll down and on the "Stack settings" check the "NodeJS Version". It’s recommended to use only latest version of the environment stack.</br> <img src="/resources/azure/appservice/nodejs-version/step5.png"/>
6. If the "App Service" is not using the latest version of NodeJS then select the latest version from the "Major version" dropdown.</br> <img src="/resources/azure/appservice/nodejs-version/step6.png"/>
7. Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/appservice/nodejs-version/step7.png"/>
8. Click "Continue" in the confirmation pop up to save the changes.</br> <img src="/resources/azure/appservice/nodejs-version/step8.png"/>
9. Repeat steps number 3 - 8 to verify all other "Apps" are using latest Stack version in the account.</br>
