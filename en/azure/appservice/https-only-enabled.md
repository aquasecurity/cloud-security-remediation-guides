[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / App Service / HTTPS Only Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | HTTPS Only Enabled |
| **Cloud** | AZURE |
| **Category** | App Service |
| **Description** | Ensures HTTPS Only is enabled for App Services, redirecting all HTTP traffic to HTTPS |
| **More Info** | Enabling HTTPS Only traffic will redirect all non-secure HTTP requests to HTTPS. HTTPS uses the SSL/TLS protocol to provide a secure connection. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/app-service/app-service-web-tutorial-custom-ssl#enforce-https |
| **Recommended Action** | Enable HTTPS Only support SSL settings for all App Services |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for App Services. </br> <img src="/resources/azure/appservice/https-only-enabled/step2.png"/>
3. Select the "App Services" by clicking on the "Name" link to access the configuration changes.</br> <img src="/resources/azure/appservice/https-only-enabled/step3.png"/>
4. Scroll down the selected "App Services" navigation panel and in "Settings" click on the "TLS/SSL settings" option.</br> <img src="/resources/azure/appservice/https-only-enabled/step4.png"/>	
5. On the "TLS/SSL settings" page check if "HTTPS Only" is "ON/OFF". If it's turned "OFF" then it will not redirect all non-secure HTTP requests to HTTPS. </br> <img src="/resources/azure/appservice/https-only-enabled/step5.png"/>	
6. Repeat steps number 2 - 5 to verify other "Apps" SSL settings in the account.</br>	
7. Navigate to the "App Services", select the "App Service" and click on the "Name" as a link to access the configuration, select the "TLS/SSL settings" under "Settings."</br>	<img src="/resources/azure/appservice/https-only-enabled/step7.png"/>	
8. On the "Protocol Settings" page click on the "ON" option next to "HTTPS Only" which will redirect all non-secure HTTP requests to HTTPS. HTTPS uses the SSL/TLS protocol to provide a secure connection.</br> <img src="/resources/azure/appservice/https-only-enabled/step8.png"/>	
9. Repeat above steps to ensures "HTTPS Only" are enabled for "App Services",ensures HTTPS Only is enabled for your App services, redirecting all HTTP traffic to HTTPS.</br> 
