[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Security Center / Monitor System Updates

## Quick Info

| | |
|-|-|
| **Plugin Title** | Monitor System Updates |
| **Cloud** | AZURE |
| **Category** | Security Center |
| **Description** | Ensures that Monitor System Updates is enabled in Security Center |
| **More Info** | When this setting is enabled, Security Center will audit virtual machines for pending OS or system updates. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-policy-definitions |
| **Recommended Action** | Ensure System Update monitoring is configured for virtual machines from the Azure Security Center. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Security Center. </br> <img src="/resources/azure/securitycenter/monitor-system-updates/step2.png"/>
3. Scroll down the "Security Center" and select the "Security policy" option under "Management" in the left navigation panel.</br>
4. On the "Policy Management" page under "Name" column select the "Subscription Name" that needs to be verified.</br> <img src="/resources/azure/securitycenter/monitor-system-updates/step4.png"/>
5. In the "Security Policy" page scroll down and click on the "Azure Security Benchmark".</br> <img src="/resources/azure/securitycenter/monitor-system-updates/step5.png"/>
6. In the "Azure Security Benchmark" click on the Next button.</br> <img src="/resources/azure/securitycenter/monitor-system-updates/step6.png"/>
7. In the "Azure Security Benchmark", check for the "System updates should be installed on your machines" Parameter and if it's set to "Disable" then the encryption is not enabled.</br> <img src="/resources/azure/securitycenter/monitor-system-updates/step7.png"/>
8. Repeat steps number 2 - 7 to check other "Subscriptions" under the "Security Center."</br>
9. Navigate to the "Security Center", select the "Security policy" and under "Policy Management" select the "Subscription" that needs to enable the "Monitor System Updates."</br> <img src="/resources/azure/securitycenter/monitor-system-updates/step9.png"/>
10. Select the "Subscription" link under the "Security policy" at the top to get into the configuration settings. </br> <img src="/resources/azure/securitycenter/monitor-system-updates/step10.png"/>
11. Scroll down the page and under "Parameter" choose the "System updates should be installed on your machines" and select the "AuditIfNotExists" option from the dropdown menu and click on the "Save" button at the bottom to make the necessary changes.</br> <img src="/resources/azure/securitycenter/monitor-system-updates/step11.png"/>
12. Repeat steps number 9 - 11 to ensure System Update monitoring is configured for virtual machines from the Azure Security Center.</br>
