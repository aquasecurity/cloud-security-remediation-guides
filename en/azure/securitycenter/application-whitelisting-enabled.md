[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Security Center / Application Whitelisting Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Application Whitelisting Enabled |
| **Cloud** | AZURE |
| **Category** | Security Center |
| **Description** | Ensures that Security Center Monitor Adaptive Application Whitelisting is enabled |
| **More Info** | Adaptive application controls work in conjunction with machine learning to analyze processes running in a VM and help control which applications can run, hardening the VM against malware. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-adaptiveapplication |
| **Recommended Action** | Enable Adaptive Application Controls for Virtual Machines from the Azure Security Center by ensuring AuditIfNotExists setting is used. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Microsoft Defender for Cloud". </br> <img src="/resources/azure/securitycenter/application-whitelisting-enabled/step2.png"/>
3. Scroll down the left navigation panel and select the "Environment Settings" under "Management".</br> <img src="/resources/azure/securitycenter/application-whitelisting-enabled/step3.png"/>
4. On the "Microsoft Defender for Cloud | Environment settings" page under "Name" column, select the "Subscription Name" that needs to be verified by clicking on its Name.</br> <img src="/resources/azure/securitycenter/application-whitelisting-enabled/step4.png"/>
5. On the "Settings" page scroll down the "Policy settings" section and select "Security Policy".</br> <img src="/resources/azure/securitycenter/application-whitelisting-enabled/step5.png"/>
6. On the "Settings | Security policy" page, Select the "Subscription" link under the "Security policy" at the top to get into the configuration settings. </br> <img src="/resources/azure/securitycenter/application-whitelisting-enabled/step6.png"/>
7. On the Settings page, select the "Parameters" tab and uncheck "Only show parameters that need input or review". It will show you a list of parameters.</br> <img src="/resources/azure/securitycenter/application-whitelisting-enabled/step7.png"/>
8. In the list search for the setting "Adaptive Application Controls for defining safe applications should be enabled on your machines". If it's set to "Disabled" then "Adaptive Application Whitelisting" is not enabled on the selected "Subscription".</br> <img src="/resources/azure/securitycenter/application-whitelisting-enabled/step8.png"/>
9. To enable ""Adaptive Application Whitelisting" click to open the dropdown of "Adaptive Application Controls should be enabled on virtual machines" and select the "AuditIfNotExists" option. Click on the "Review + save" button at the bottom. </br> <img src="/resources/azure/securitycenter/application-whitelisting-enabled/step9.png"/>
10. On the "Review + save" page, click on "Save" button to make the necessary changes.</br> <img src="/resources/azure/securitycenter/application-whitelisting-enabled/step10.png"/>
11. Repeat step number 3 - 10 to ensures "Adaptive Application Whitelisting" is enabled for Subscriptions.</br>
