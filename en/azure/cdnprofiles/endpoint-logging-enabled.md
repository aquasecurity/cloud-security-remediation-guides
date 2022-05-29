[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / CDN Profiles / Endpoint Logging Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Endpoint Logging Enabled |
| **Cloud** | AZURE |
| **Category** | CDN Profiles |
| **Description** | Ensures that endpoint requests are being logged for CDN endpoints |
| **More Info** | Endpoint Logging ensures that all requests to a CDN endpoint are logged. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/cdn/cdn-azure-diagnostic-logs |
| **Recommended Action** | Ensure that diagnostic logging is enabled for each CDN endpoint for each CDN profile |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for CDN. Select "Front Door and CDN profiles".</br> <img src="/resources/azure/cdnprofiles/endpoint-logging-enabled/step2.png"/>
3. On the “Front Door and CDN profiles” page, click on the “Name” link to access the configuration changes.</br> <img src="/resources/azure/cdnprofiles/endpoint-logging-enabled/step3.png"/>
4. In the left navigation panel, click on the "Diagnostic setting" under "Monitoring".</br> <img src="/resources/azure/cdnprofiles/endpoint-logging-enabled/step4.png"/>
5. In the "Diagnostic setting" panel if you see "No diagnostic settings defined" then logging is not enabled for this CDN. This is against the Azure best practices. Now click on the "+ Add diagnostic setting" link to enable diagnostic logging.</br> <img src="/resources/azure/cdnprofiles/endpoint-logging-enabled/step5.png"/>
6. On the "Diagnostic setting" page that opens select "all logs" under "Logs".</br> <img src="/resources/azure/cdnprofiles/endpoint-logging-enabled/step6.png"/>
7. Under "Metrics" select "AllMetrics. </br> <img src="/resources/azure/cdnprofiles/endpoint-logging-enabled/step7.png"/>
8. Under "Destination details" select "Send to Log Analytics workspace".</br> <img src="/resources/azure/cdnprofiles/endpoint-logging-enabled/step8.png"/>
9. Click "Save" at the top of the page to save the changes and enable logging.</br> <img src="/resources/azure/cdnprofiles/endpoint-logging-enabled/step9.png"/>
10. Repeat steps 3 - 9 for all other CDN endpoints.

