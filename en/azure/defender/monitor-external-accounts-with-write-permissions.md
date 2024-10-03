[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Defender / Monitor External Accounts with Write Permissions

## Quick Info

| |                                                                                                                |
|-|----------------------------------------------------------------------------------------------------------------|
| **Plugin Title** | Monitor External Accounts with Write Permissions                                                               |
| **Cloud** | AZURE                                                                                                          |
| **Category** | Defender                                                                                                       |
| **Description** | Ensures that External Accounts with Write Permissions are being Monitored in Microsoft Defender.                                                    |
| **More Info** | External Accounts with Write Permissions should be monitored to meet you organization's security compliance requirements. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/defender-for-cloud/policy-reference               |
| **Recommended Action** | Enable Monitor for External Accounts with Write Permissions by ensuring AuditIfNotExists setting is used for 'External accounts with write permissions should be removed from your subscription' from the Microsoft Defender.                              |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Policy" and select the "Policy". </br> <img src="/resources/azure/defender/monitor-external-accounts-with-write-permissions/step2.png"/>
3. Scroll down the left navigation panel and select "Compliance".</br> <img src="/resources/azure/defender/monitor-external-accounts-with-write-permissions/step3.png"/>
4. On the "Policy | Compliance" page, under "Name" column select compliance for the "Scope" of necessary Subscription.</br> <img src="/resources/azure/defender/monitor-external-accounts-with-write-permissions/step4.png"/>
5. On the "Policy| Compliance" page select the "View Assignment" Tab on the top. </br> <img src="/resources/azure/defender/monitor-external-accounts-with-write-permissions/step5.png"/>
6. On the "Policy| Compliance | Subscription" page, Select the "Edit Assignment" Tab at the top.</br> <img src="/resources/azure/defender/monitor-external-accounts-with-write-permissions/step6.png"/>
7. On the Assign Initiative page, select the "Parameters" tab and uncheck "Only show parameters that need input or review". It will show you a list of parameters.</br>  <img src="/resources/azure/defender/monitor-external-accounts-with-write-permissions/step7.png"/>
8. In the list search for the setting "External accounts with write permissions should be removed from your subscription". If it's set to "Disabled" then "External accounts Monitoring" is not enabled on the selected "Subscription".</br> <img src="/resources/azure/defender/monitor-external-accounts-with-write-permissions/step8.png"/>
9. To enable "External accounts Monitoring" click to open the dropdown of "External accounts with write permissions should be removed from your subscription" and select the "AuditIfNotExists" option.</br> <img src="/resources/azure/defender/monitor-external-accounts-with-write-permissions/step9.png"/>
10. Click on the "Review + save" button to make the necessary changes.</br> <img src="/resources/azure/defender/monitor-external-accounts-with-write-permissions/step10.png"/>
11. Repeat steps number 3 - 10 to ensure ""External accounts Monitoring" is configured from the Azure Defender.</br>
