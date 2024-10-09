[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Defender /  Monitor Next Generation Firewall 

## Quick Info

| | |
|-|------------------------------------------------------------------------------------------------------------------------------------|
| **Plugin Title** | Monitor Next Generation Firewall |
| **Cloud** | AZURE |
| **Category** | Defender |
| **Description** | Ensures that Next Generation Firewall (NGFW) Monitoring is enabled in Microsoft Defender. |
| **More Info** | When this setting is enabled, Microsoft Defender for Cloud will search for deployments where a NGFW is recommended. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/defender-for-cloud/policy-reference |
| **Recommended Action** | Enable Next Generation Firewall Monitoring by ensuring AuditIfNotExists setting is used for 'All network ports should be restricted on network security groups associated to your virtual machine' from the Microsoft Defender. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Policy" and select the "Policy". </br> <img src="/resources/azure/defender/monitor-next-generation-firewall/step2.png"/>
3. Scroll down the left navigation panel and select "Compliance". </br> <img src="/resources/azure/defender/monitor-next-generation-firewall/step3.png"/>
4. On the "Policy | Compliance" page, under "Name" column select compliance for the "Scope" of necessary Subscription. </br> <img src="/resources/azure/defender/monitor-next-generation-firewall/step4.png"/>
5. On the "Policy| Compliance" page select the "View Assignment" Tab on the top. </br> <img src="/resources/azure/defender/monitor-next-generation-firewall/step5.png"/>
6. On the "Policy| Compliance | Subscription" page, Select the "Edit Assignment" Tab at the top. </br> <img src="/resources/azure/defender/monitor-next-generation-firewall/step6.png"/>
7. On the Assign Initiative page, select the "Parameters" tab and uncheck "Only show parameters that need input or review". It will show you a list of parameters. </br>  <img src="/resources/azure/defender/monitor-next-generation-firewall/step7.png"/>
8. In the list search for the setting "All Internet traffic should be routed via your deployed Azure Firewall". If it's set to "Disabled" then "Next Generation Firewall Monitoring" is not enabled on the selected "Subscription". </br> <img src="/resources/azure/defender/monitor-next-generation-firewall/step8.png"/>
9. To enable "Next Generation Firewall Monitoring" click to open the dropdown of "All Internet traffic should be routed via your deployed Azure Firewall" and select the "AuditIfNotExists" option. </br> <img src="/resources/azure/defender/monitor-next-generation-firewall/step9.png"/>
10. Click on the "Review + save" button to make the necessary changes. </br> <img src="/resources/azure/defender/monitor-next-generation-firewall/step10.png"/>
11. Repeat steps number 3 - 10 to ensure "Next Generation Firewall Monitoring" is configured from the Azure Defender. </br>
