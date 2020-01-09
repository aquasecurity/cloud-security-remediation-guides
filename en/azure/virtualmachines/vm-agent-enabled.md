[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Virtual Machines / VM Agent Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | VM Agent Enabled |
| **Cloud** | AZURE |
| **Category** | Virtual Machines |
| **Description** | Ensures that the VM Agent is enabled for virtual machines |
| **More Info** | The VM agent must be enabled on Azure virtual machines in order to enable Azure Security Center for data collection. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-enable-vm-agent |
| **Recommended Action** | Enable the VM agent for all virtual machines. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Security Center. </br> <img src="/resources/azure/virtualmachines/vm-agent-enabled/step2.png"/>
3. Click on the "Pricing & Settings" option and choose the "Subscription" and click on the "Name" option as a link to access the configurations. </br> <img src="/resources/azure/virtualmachines/vm-agent-enabled/step3.png"/>
4. Click on the "Data Collection" option under Settings. </br> <img src="/resources/azure/virtualmachines/vm-agent-enabled/step4.png"/>
5. Under the "Data Colelction" check whether the "Auto Provisioning" is "ON or OFF". If "Auto Provisioning" is turned "Off" then the automatic installation of the Microsoft Monitoring Agent on all the VMs in your subscription is not enabled. </br> <img src="/resources/azure/virtualmachines/vm-agent-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify "VM Agent" in the other Azure accounts.</br>
7. Navigate to the "Security Center", select the "Price & Settings" and click on the "Subscription Name", select the "Data Collection" options under "Settings".</br> <img src="/resources/azure/virtualmachines/vm-agent-enabled/step7.png"/>
8. Turn "On" the "Auto Provisioning" feature and click on the "Save" button at the top to make the changes. Once enabled, any new or existing VM without an installed Microsoft Monitoring agent (MMA) extension, will have it provisioned. </br> <img src="/resources/azure/virtualmachines/vm-agent-enabled/step8.png"/>
9. Repeat steps number 7 - 8 to enable the VM agent for all virtual machines.</br>
