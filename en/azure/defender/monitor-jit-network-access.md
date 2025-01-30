[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Defender / Monitor JIT Network Access

## Quick Info

| | |
|-|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Plugin Title** | Monitor JIT Network Access |
| **Cloud** | AZURE |
| **Category** | Defender |
| **Description** | Ensures Just In Time Network Access monitoring is enabled in Defender |
| **More Info** | When this setting is enabled, Defender audits Just In Time Network Access on all virtual machines (Windows and Linux as well) to enhance data protection at rest |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/defender-for-cloud/policy-reference |
| **Recommended Action** | Ensure JIT Network Access monitoring is configured for compute and apps from the Azure Defender. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Policy" and select the "Policy". </br> <img src="/resources/azure/defender/monitor-jit-network-access/step2.png"/>
3. Scroll down the left navigation panel and select "Compliance". </br> <img src="/resources/azure/defender/monitor-jit-network-access/step3.png"/>
4. On the "Policy | Compliance" page, under "Name" column select compliance for the "Scope" of necessary Subscription. </br> <img src="/resources/azure/defender/monitor-jit-network-access/step4.png"/>
5. On the "Policy| Compliance" page select the "View Assignment" Tab on the top. </br> <img src="/resources/azure/defender/monitor-jit-network-access/step5.png"/>
6. On the "Policy| Compliance | Subscription" page, Select the "Edit Assignment" Tab at the top. </br> <img src="/resources/azure/defender/monitor-jit-network-access/step6.png"/>
7. On the Assign Initiative page, select the "Parameters" tab and uncheck "Only show parameters that need input or review". It will show you a list of parameters. </br>  <img src="/resources/azure/defender/monitor-jit-network-access/step7.png"/>
8. In the list search for the setting "Management ports of virtual machines should be protected with just-in-time network access control". If it's set to "Disabled" then "JIT Network Access monitoring" is not enabled on the selected "Subscription". </br> <img src="/resources/azure/defender/monitor-jit-network-access/step8.png"/>
9. To enable "JIT Network Access monitoring" click to open the dropdown of "Management ports of virtual machines should be protected with just-in-time network access control" and select the "AuditIfNotExists" option. </br> <img src="/resources/azure/defender/monitor-jit-network-access/step9.png"/>
10. Click on the "Review + save" button to make the necessary changes. </br> <img src="/resources/azure/defender/monitor-jit-network-access/step10.png"/>
11. Repeat steps number 3 - 10 to ensure "Monitor JIT Network Access" is configured from the Azure Defender. </br>
