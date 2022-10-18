[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Security Center / Security Configuration Monitoring

## Quick Info

| | |
|-|-|
| **Plugin Title** | Security Configuration Monitoring |
| **Cloud** | AZURE |
| **Category** | Security Center |
| **Description** | Ensures that Security Configuration Monitoring is enabled in Security Center |
| **More Info** | When this setting is enabled, Security Center will monitor virtual machines for security configurations. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/governance/policy/overview |
| **Recommended Action** | Ensure Security Configuration Monitoring is configured for virtual machines from the Azure Security Center. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Microsoft Defender for Cloud". </br> <img src="/resources/azure/securitycenter/security-configuration-monitoring/step2.png"/>
3. Scroll down the left navigation panel and select the "Environment Settings" under "Management".</br> <img src="/resources/azure/securitycenter/security-configuration-monitoring/step3.png"/>
4. On the "Microsoft Defender for Cloud | Environment settings" page under "Name" column select the "Subscription Name" that needs to be verified by clicking on its Name.</br> <img src="/resources/azure/securitycenter/security-configuration-monitoring/step4.png"/>
5. On the "Settings" page scroll down the "Policy settings" section and select "Security Policy".</br> <img src="/resources/azure/securitycenter/security-configuration-monitoring/step5.png"/>
6. On the "Settings | Security policy" page, Select the "Subscription" link under the "Security policy" at the top to get into the configuration settings.</br> <img src="/resources/azure/securitycenter/security-configuration-monitoring/step6.png"/>
7. On the Settings page, select the "Parameters" tab and uncheck "Only show parameters that need input or review". It will show you a list of parameters.</br>  <img src="/resources/azure/securitycenter/security-configuration-monitoring/step7.png"/>
8. In the list search for the setting "Vulnerabilities in security configuration on your machines should be remediated". If it's set to "Disabled" then "Security Configuration Monitoring" is not enabled on the selected "Subscription".</br> <img src="/resources/azure/securitycenter/security-configuration-monitoring/step8.png"/>
9. To enable "Security Configuration Monitoring" click to open the dropdown of "Vulnerabilities in security configuration on your machines should be remediated" and select the "AuditIfNotExists" option. Click on the "Review + save" button at the bottom.</br> <img src="/resources/azure/securitycenter/security-configuration-monitoring/step9.png"/>
10. On the "Review + save" page, click on "Save" button to make the necessary changes.</br> <img src="/resources/azure/securitycenter/security-configuration-monitoring/step10.png"/>
11. Repeat step number 3 - 10 to ensure Security Configuration Monitoring is configured from the Azure Security Center.</br>
