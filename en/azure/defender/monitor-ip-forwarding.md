[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Defender / Monitor IP Forwarding

## Quick Info

| | |
|-|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Plugin Title** | Monitor IP Forwarding|
| **Cloud** | AZURE |
| **Category** | Defender |
| **Description** | Ensures that Virtual Machine IP Forwarding Monitoring is enabled in Microsoft Defender. |
| **More Info** | IP Forwarding feature should be monitored to meet you organization's security compliance requirements. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/defender-for-cloud/policy-reference |
| **Recommended Action** | Enable IP Forwarding Monitoring by ensuring AuditIfNotExists setting is used for 'IP Forwarding on your virtual machine should be disabled' from the Microsoft Defender. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Policy" and select the "Policy". </br> <img src="/resources/azure/defender/monitor-ip-forwarding/step2.png"/>
3. Scroll down the left navigation panel and select "Compliance". </br> <img src="/resources/azure/defender/monitor-ip-forwarding/step3.png"/>
4. On the "Policy | Compliance" page, under "Name" column select compliance for the "Scope" of necessary Subscription. </br> <img src="/resources/azure/defender/monitor-ip-forwarding/step4.png"/>
5. On the "Policy| Compliance" page select the "View Assignment" Tab on the top. </br> <img src="/resources/azure/defender/monitor-ip-forwarding/step5.png"/>
6. On the "Policy| Compliance | Subscription" page, Select the "Edit Assignment" Tab at the top. </br> <img src="/resources/azure/defender/monitor-ip-forwarding/step6.png"/>
7. On the Assign Initiative page, select the "Parameters" tab and uncheck "Only show parameters that need input or review". It will show you a list of parameters. </br>  <img src="/resources/azure/defender/monitor-ip-forwarding/step7.png"/>
8. In the list search for the setting "IP Forwarding on your virtual machine should be disabled". If it's set to "Disabled" then "IP Forwarding Monitoring" is not enabled on the selected "Subscription". </br> <img src="/resources/azure/defender/monitor-ip-forwarding/step8.png"/>
9. To enable "IP Forwarding Monitoring" click to open the dropdown of "IP Forwarding on your virtual machine should be disabled" and select the "AuditIfNotExists" option. </br> <img src="/resources/azure/defender/monitor-ip-forwarding/step9.png"/>
10. Click on the "Review + save" button to make the necessary changes. </br> <img src="/resources/azure/defender/monitor-ip-forwarding/step10.png"/>
11. Repeat steps number 3 - 10 to ensure "IP Forwarding Monitoring" is configured from the Azure Defender.</br>
