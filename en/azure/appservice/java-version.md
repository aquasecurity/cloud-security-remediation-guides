[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / App Service / Java Version

## Quick Info

| | |
|-|-|
| **Plugin Title** | Java Version |
| **Cloud** | AZURE |
| **Category** | App Service |
| **Description** | Ensures the latest version of Java is installed for all App Services |
| **More Info** | Installing the latest version of Java will reduce the security risk of missing security patches. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/app-service/app-service-web-get-started-java |
| **Recommended Action** | Select the latest version of Java for all Java-based App Services |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Find the search bar at the top and search for App Services. </br> <img src="/resources/azure/appservice/.net-framework-version/step2.png"/>
3. Select the "App Service" by clicking on "Name" to go to its configuration.</br> <img src="/resources/azure/appservice/.net-framework-version/step3.png"/>
4. Scroll down the selected "App Services" left navigation panel and in "Settings" click on the "Configuration" option.</br <img src="/resources/azure/appservice/.net-framework-version/step4.png"/>
5. On the "Configuration" page select the General settings tab, scroll down and on the "Stack settings" check the ".NET Framework Version". It’s recommended to use only latest version of the environment stack.</br> <img src="/resources/azure/appservice/.net-framework-version/step5.png"/>
6. If the "App Service" is not using the latest version of the .NET Framework then select the latest version from the ".NET version" dropdown.</br> <img src="/resources/azure/appservice/.net-framework-version/step6.png"/>
7. Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/appservice/.net-framework-version/step7.png"/>
8. Click "Continue" in the confirmation pop up to save the changes.</br> <img src="/resources/azure/appservice/.net-framework-version/step8.png"/>
9. Repeat steps number 3 - 7 to verify all other "Apps" are using latest Stack version in the account.</br>
