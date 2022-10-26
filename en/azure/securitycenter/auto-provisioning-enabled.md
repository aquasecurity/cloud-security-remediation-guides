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

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Microsoft Defender for Cloud". </br> <img src="/resources/azure/securitycenter/auto-provisioning-enabled/step2.png"/>
3. On the "Microsoft Defender for Cloud" page scroll down the left navigation panel and choose "Environment Settings".</br> <img src="/resources/azure/securitycenter/auto-provisioning-enabled/step3.png"/>
4. On the "Environment Settings" page, select the "Subscription" by clicking on its "Name".</br> <img src="/resources/azure/securitycenter/auto-provisioning-enabled/step4.png"/>
5. Under the "Settings" page, click on "Auto Provisioning" </br> <img src="/resources/azure/securitycenter/auto-provisioning-enabled/step5.png"/>
6. On the "Settings | Auto provisioning" page, if the "Log Analytics agent for Azure VMs" shows status as turned off, then the "Automatic provisioning" of the monitoring agent is not enabled.</br> <img src="/resources/azure/securitycenter/auto-provisioning-enabled/step6.png"/>
7. On the "Settings | Auto provisioning" page, turn the status "ON" for "Log Analytics agent for Azure VMs" by toggling it.</br> <img src="/resources/azure/securitycenter/auto-provisioning-enabled/step7.png"/>
8. To the right under "Configuration" click on "Edit configuration". </br> <img src="/resources/azure/securitycenter/auto-provisioning-enabled/step8.png"/>
9. On the "Extension deployment configuration" page, select the "Workspace configuration" and click on the "All Events" under the "Windows security events". Click on the "Apply" button to make the changes.</br> <img src="/resources/azure/securitycenter/auto-provisioning-enabled/step9.png"/>
10. Repeat step number 3 - 9 to ensure that the data collection settings of the subscription have Auto Provisioning set to enabled.</br>
