[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Defender / Security Configuration Monitoring

## Quick Info

| |                                                                                                                       |
|-|-----------------------------------------------------------------------------------------------------------------------|
| **Plugin Title** | Security Configuration Monitoring                                                                                     |
| **Cloud** | AZURE                                                                                                                 |
| **Category** | Defender                                                                                                              |
| **Description** | Ensures that Security Configuration Monitoring is enabled in Microsoft Defender.                                      |
| **More Info** | When this setting is enabled, Microsoft Defender for Cloud will monitor virtual machines for security configurations. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/governance/policy/overview                                                    |
| **Recommended Action** | Ensure Security Configuration Monitoring is configured for virtual machines from Microsoft Defender.                  |

## Detailed Remediation Steps
1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Microsoft Defender for Cloud". </br> <img src="/resources/azure/defender/security-configuration-monitoring/step2.png"/>
3. Scroll down the left navigation panel and select "Environment Settings" under "Management".</br> <img src="/resources/azure/defender/security-configuration-monitoring/step3.png"/>
4. On the "Microsoft Defender for Cloud | Environment settings" page, under the "Name" column, select the "Subscription Name" that needs to be verified by clicking on its Name.</br> <img src="/resources/azure/defender/security-configuration-monitoring/step4.png"/>
5. On the "Settings" page, Defender Plans. Select the "Settings & Monitoring" Tab on the top.</br> <img src="/resources/azure/defender/security-configuration-monitoring/step5.png"/>
6. On the "Settings | Defender plans" page, Navigate to the "Guest Configuration agent" plan.</br> <img src="/resources/azure/defender/security-configuration-monitoring/step6.png"/>
7. Enable the "Guest Configuration agent" by toggling its Status to "On".</br>  <img src="/resources/azure/defender/security-configuration-monitoring/step7.png"/>
8. On the "Settings & Monitoring" Page, click on the "Continue" Button at the top.</br>  <img src="/resources/azure/defender/security-configuration-monitoring/step8.png"/>
9. On the "Settings | Defender plans" Page, click on the "Save" Button at the top.</br>  <img src="/resources/azure/defender/security-configuration-monitoring/step9.png"/>
10. Repeat steps 3 - 9 to ensure Security Configuration Monitoring is configured from Microsoft Defender for Cloud.</br>
