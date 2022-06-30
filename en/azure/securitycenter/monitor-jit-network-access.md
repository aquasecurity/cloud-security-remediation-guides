[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Security Center / Monitor JIT Network Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Monitor JIT Network Access |
| **Cloud** | AZURE |
| **Category** | Security Center |
| **Description** | Ensures Just In Time Network Access monitoring is enabled in Security Center |
| **More Info** | When this setting is enabled, Security Center audits Just In Time Network Access on all virtual machines (Windows and Linux as well) to enhance data protection at rest |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-policy-definitions |
| **Recommended Action** | Ensure JIT Network Access monitoring is configured for compute and apps from the Azure Security Center. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Microsoft Defender for Cloud". </br> <img src="/resources/azure/securitycenter/monitor-jit-network-access/step2.png"/>
3. Scroll down the left navigation panel and select the "Environment Settings" under "Management".</br> <img src="/resources/azure/securitycenter/monitor-jit-network-access/step3.png"/>
4. On the "Microsoft Defender for Cloud | Environment settings" page under "Name" column select the "Subscription Name" that needs to be verified by clicking on its Name.</br> <img src="/resources/azure/securitycenter/monitor-jit-network-access/step4.png"/>
5. On the "Settings" page scroll down the "Policy settings" section and select "Security Policy".</br> <img src="/resources/azure/securitycenter/monitor-jit-network-access/step5.png"/>
6. On the "Settings | Security policy" page, Select the "Subscription" link under the "Security policy" at the top to get into the configuration settings.</br> <img src="/resources/azure/securitycenter/monitor-jit-network-access/step6.png"/>
7. On the Settings page, select the "Parameters" tab and uncheck "Only show parameters that need input or review". It will show you a list of parameters.</br>  <img src="/resources/azure/securitycenter/monitor-jit-network-access/step7.png"/>
8. In the list search for the setting "Management ports of virtual machines should be protected with Just-In-Time network access control". If it's set to "Disabled" then "Disk Encryption monitoring" is not enabled on the selected "Subscription".</br> <img src="/resources/azure/securitycenter/monitor-jit-network-access/step8.png"/>
9. To enable "JIT Network Access monitoring" click to open the dropdown of "Management ports of virtual machines should be protected with Just-In-Time network access control" and select the "AuditIfNotExists" option. Click on the "Review + save" button at the bottom.</br> <img src="/resources/azure/securitycenter/monitor-jit-network-access/step9.png"/>
10. On the "Review + save" page, click on "Save" button to make the necessary changes.</br> <img src="/resources/azure/securitycenter/monitor-jit-network-access/step10.png"/>
11. Repeat steps number 3 - 10 to ensure ensure JIT Network Access monitoring is configured for compute and apps from the Azure Security Center</br>
