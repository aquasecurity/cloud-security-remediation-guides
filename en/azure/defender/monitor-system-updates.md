[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Defender / Monitor System Updates

## Quick Info

| |                                                                                                      |
|-|------------------------------------------------------------------------------------------------------|
| **Plugin Title** | Monitor System Updates                                                                               |
| **Cloud** | AZURE                                                                                                |
| **Category** | Defender                                                                                             |
| **Description** | Ensures that Monitor System Updates is enabled in Defender                                           |
| **More Info** | When this setting is enabled, Defender will audit virtual machines for pending OS or system updates. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/defender-for-cloud/policy-reference            |
| **Recommended Action** | Ensure System Update monitoring is configured for virtual machines from the Microsoft Defender.      |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Policy" and select the "Policy". </br> <img src="/resources/azure/defender/monitor-system-updates/step2.png"/>
3. Scroll down the left navigation panel and select "Compliance".</br> <img src="/resources/azure/defender/monitor-system-updates/step3.png"/>
4. On the "Policy | Compliance" page, under "Name" column select compliance for the "Scope" of necessary Subscription.</br> <img src="/resources/azure/defender/monitor-system-updates/step4.png"/>
5. On the "Policy| Compliance" page select the "View Assignment" Tab on the top. </br> <img src="/resources/azure/defender/monitor-system-updates/step5.png"/>
6. On the "Policy| Compliance | Subscription" page, Select the "Edit Assignment" Tab at the top.</br> <img src="/resources/azure/defender/monitor-system-updates/step6.png"/>
7. On the Assign Initiative page, select the "Parameters" tab and uncheck "Only show parameters that need input or review". It will show you a list of parameters.</br>  <img src="/resources/azure/defender/monitor-system-updates/step7.png"/>
8. In the list search for the setting "System updates should be installed on your machines". If it's set to "Disabled" then "System Update monitoring" is not enabled on the selected "Subscription".</br> <img src="/resources/azure/defender/monitor-system-updates/step8.png"/>
9. To enable "System Update monitoring" click to open the dropdown of "System updates should be installed on your machines" and select the "AuditIfNotExists" option.</br> <img src="/resources/azure/defender/monitor-system-updates/step9.png"/>
10. Click on the "Review + save" button to make the necessary changes.</br> <img src="/resources/azure/defender/monitor-system-updates/step10.png"/>
11. Repeat steps number 3 - 10 to ensure "System Update monitoring" is configured from the Azure Defender.</br>
