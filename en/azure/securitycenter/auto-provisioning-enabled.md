[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Security Center / Auto Provisioning Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Auto Provisioning Enabled |
| **Cloud** | AZURE |
| **Category** | Security Center |
| **Description** | Ensures that automatic provisioning of the monitoring agent is enabled |
| **More Info** | The Microsoft Monitoring Agent scans for various security-related configurations and events such as system updates, OS vulnerabilities, and endpoint protection and provides alerts. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-enable-data-collection |
| **Recommended Action** | Ensure that the data collection settings of the subscription have Auto Provisioning set to enabled. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Security Center. </br> <img src="/resources/azure/securitycenter/auto-provisioning-enabled/step2.png"/>
3. On the "Security Center" page scroll down the left navigation panel and choose "Pricing and Settings."</br> <img src="/resources/azure/securitycenter/auto-provisioning-enabled/step3.png"/>
4. On the "Security Center - Pricing & settings" page, select the "Subscription" by clicking on the "Name."</br> <img src="/resources/azure/securitycenter/auto-provisioning-enabled/step4.png"/>
5. Under the "Settings - Pricing tier", click on the "Data Collection" options and if the "Auto Provisioning" is turned off then the "Automatic provisioning" of the monitoring agent is not enable.</br> <img src="/resources/azure/securitycenter/auto-provisioning-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other Azure accounts for "Auto Provisioning Enabled."</br>
7. Navigate to Security center, choose "Pricing and Settings", select the "Subscription" by clicking on the "Name" and click on the "Data Collection" options.</br> <img src="/resources/azure/securitycenter/auto-provisioning-enabled/step7.png"/>
8. On the "Settings - Data Collection" page, click on the "ON" option next to the "Auto Provisioning."</br> <img src="/resources/azure/securitycenter/auto-provisioning-enabled/step8.png"/>
9. On the "Settings - Data Collection" page, select the "Workspace configuration" and click on the "All Events" under the "Windows security events". Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/securitycenter/auto-provisioning-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to ensure that the data collection settings of the subscription have Auto Provisioning set to enabled.</br>
