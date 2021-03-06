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

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for App Services. </br> <img src="/resources/azure/appservice/java-version/step2.png"/>
3. Select the "App Services" by clicking on the "Name" link to access the configuration changes.</br> <img src="/resources/azure/appservice/java-version/step3.png"/>
4. Scroll down the selected "App Services" navigation panel and in "Settings" click on the "Configuration" option.</br <img src="/resources/azure/appservice/java-version/step4.png"/>    
5. On the "Configuration" page select the General settings tab,scroll down and on the "Stack settings" check the "Java Version". It's recommended to use only latest version of the environment stack.</br> <img src="/resources/azure/appservice/java-version/step5.png"/>    
6. Repeat steps number 2 - 5 to verify other "Apps" using latest Stack version in the account.</br>    
7. Navigate to the "App Services", select the "App Service" and click on the "Name" as a link to access the configuration, select the "Configuration" under "Settings."</br> <img src="/resources/azure/appservice/java-version/step7.png"/>    
8. On the "General Settings" page scroll down and on the "Stack settings" choose the latest version of the Java from the dropdown menu and click on the "Save" button to make the changes.</br> <img src="/resources/azure/appservice/java-version/step8.png"/>    
9. Repeat above steps to ensure the latest version of Java is installed on all App Services. </br>
