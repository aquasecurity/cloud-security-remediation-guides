[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / VM Agent Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Agent Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that the VM Agent is enabled for virtual machines |
| **More Info** | The VM agent must be enabled on Azure virtual machines in order to enable Azure Defender for data collection. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/defender-for-cloud/enable-agentless-scanning-vms |
| **Recommended Action** | Enable the VM agent for all virtual machines. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Microsoft Defender for Cloud". </br> <img src="/resources/azure/virtualmachines/vm-agent-enabled/step2.png"/>
3. On the "Microsoft Defender for Cloud" page scroll down the left navigation panel and choose "Environment Settings". </br> <img src="/resources/azure/virtualmachines/vm-agent-enabled/step3.png"/>
4. On the "Environment Settings" page, select the "Subscription" by clicking on its "Name". </br> <img src="/resources/azure/virtualmachines/vm-agent-enabled/step4.png"/>
5. Under the "Settings" page, click on "Defender Plans". </br> <img src="/resources/azure/virtualmachines/vm-agent-enabled/step5.png"/>
6. Navigate to the "Server" plan in "Defender Plans" and make sure they are turned "ON". Proceed to Settings for "Server" under "Monitoring Coverage" for plans. </br> <img src="/resources/azure/virtualmachines/vm-agent-enabled/step6.png"/>
7. On the "Settings & monitoring" Page turn on "Agentless Scanning for machines".</br> <img src="/resources/azure/virtualmachines/vm-agent-enabled/step7.png"/>
8. At the top of "Settings & monitoring" Page click on "Continue" to save the changes made. </br> <img src="/resources/azure/virtualmachines/vm-agent-enabled/step8.png"/>
9. Repeat steps number 7 - 8 to enable the VM agent for all virtual machines.</br>
