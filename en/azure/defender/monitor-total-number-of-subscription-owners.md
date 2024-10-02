[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Defender / Monitor Total Number of Subscription Owners

## Quick Info

| |                                                                                                                                                   |
|-|---------------------------------------------------------------------------------------------------------------------------------------------------|
| **Plugin Title** | Monitor Total Number of Subscription Owners                                                                                                                       |
| **Cloud** | AZURE                                                                                                                                             |
| **Category** | Defender                                                                                                                                          |
| **Description** | Ensures that Total Number of Subscription Owners is being Monitored in Microsoft Defender.                                                                        |
| **More Info** | Total Number of Subscription Owners should be monitored to meet you organization's security compliance requirements. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/defender-for-cloud/policy-reference                                                         |
| **Recommended Action** | Enable Monitor for Total Number of Subscription Owners by ensuring AuditIfNotExists setting is used for 'A maximum of 3 owners should be designated for your subscription' from the Microsoft Defender.                                                                                          |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Policy" and select the "Policy". </br> <img src="/resources/azure/defender/monitor-total-number-of-subscription-owners/step2.png"/>
3. Scroll down the left navigation panel and select "Compliance".</br> <img src="/resources/azure/defender/monitor-total-number-of-subscription-owners/step3.png"/>
4. On the "Policy | Compliance" page, under "Name" column select compliance for the "Scope" of necessary Subscription.</br> <img src="/resources/azure/defender/monitor-total-number-of-subscription-owners/step4.png"/>
5. On the "Policy| Compliance" page select the "View Assignment" Tab on the top. </br> <img src="/resources/azure/defender/monitor-total-number-of-subscription-owners/step5.png"/>
6. On the "Policy| Compliance | Subscription" page, Select the "Edit Assignment" Tab at the top.</br> <img src="/resources/azure/defender/monitor-total-number-of-subscription-owners/step6.png"/>
7. On the Assign Initiative page, select the "Parameters" tab and uncheck "Only show parameters that need input or review". It will show you a list of parameters.</br>  <img src="/resources/azure/defender/monitor-total-number-of-subscription-owners/step7.png"/>
8. In the list search for the setting "A maximum of 3 owners should be designated for your subscription". If it's set to "Disabled" then "Subscription Owner Monitoring" is not enabled on the selected "Subscription".</br> <img src="/resources/azure/defender/monitor-total-number-of-subscription-owners/step8.png"/>
9. To enable "Subscription Owner Monitoring" click to open the dropdown of "A maximum of 3 owners should be designated for your subscription" and select the "AuditIfNotExists" option.</br> <img src="/resources/azure/defender/monitor-total-number-of-subscription-owners/step9.png"/>
10. Click on the "Review + save" button to make the necessary changes.</br> <img src="/resources/azure/defender/monitor-total-number-of-subscription-owners/step10.png"/>
11. Repeat steps number 3 - 10 to ensure "System Update monitoring" is configured from the Azure Defender.</br>
