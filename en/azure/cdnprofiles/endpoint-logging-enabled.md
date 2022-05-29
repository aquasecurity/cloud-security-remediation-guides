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
2. Select the "Search resources, services, and docs" option at the top and search for CDN. Select "Front Door and CDN profiles".</br> <img src="/resources/azure/cdnprofiles/detect-insecure-custom-origin/step2.png"/>
3. On the “Front Door and CDN profiles” page, click on the “Name” link to access the configuration changes.</br> <img src="/resources/azure/cdnprofiles/detect-insecure-custom-origin/step3.png"/>
4. In the CDN details pane that opens, click on the "Endpoints" link under "Properties".</br> <img src="/resources/azure/cdnprofiles/detect-insecure-custom-origin/step4.png"/>
5. On the endpoint management page that opens, click on "default-route" under "Routes" column to load the route configuration page.</br> <img src="/resources/azure/cdnprofiles/detect-insecure-custom-origin/step5.png"/>
6. On the "Update route" page, check the value of "Accepted protocols" dropdown. If it is set to "HTTP only" or "HTTP and HTTPS" then the endpoint allows insecure traffic. This is a security threat.</br> <img src="/resources/azure/cdnprofiles/detect-insecure-custom-origin/step6.png"/>
7. Click on the "Accepted protocols" dropdown and select "HTTPS only". This will configure the endpoint to accept only secure traffic.
8. Ensure that the checkbox is selected for "Redirect" to "Redirect all traffic to use HTTPS".</br> <img src="/resources/azure/cdnprofiles/detect-insecure-custom-origin/step7.png"/>
9. Click "Update" at the bottom of the page to save the changes.
10. Repeat steps 4 - 9 for all other CDN endpoints.


