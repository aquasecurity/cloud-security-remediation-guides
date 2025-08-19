[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / defender / Defender For DNS

## Quick Info

| | |
|-|-|
| **Plugin Title** | Enable Defender For DNS |
| **Cloud** | AZURE |
| **Category** | Security |
| **Description** | Ensures that Microsoft Defender for DNS is enabled. |
| **More Info** | Turning on Microsoft Defender for DNS enables threat detection, providing threat intelligence, anomaly detection, and behavior analytics in the Microsoft Defender for Cloud. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/defender-for-cloud/enable-enhanced-security |
| **Recommended Action** | Enable Microsoft Defender for Containers in Defender plans for the subscription. |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Microsoft Defender. </br> <img src="/resources/azure/defender/enable-defender-for-dns/step2.png"/>
3. On the "Microsoft Defender" page, scroll down the left navigation panel and choose "Envoirnment settings" under the "Management" section.</br> <img src="/resources/azure/defender/enable-defender-for-dns/step3.png"/>
4. On the "Envoirnment Settings" page select the subscription or workspace that you want to protect from list on bottom of page.</br> <img src="/resources/azure/defender/enable-defender-for-dns/step4.png"/>
5. On Defender plans page find the "DNS" from list and change the status "On" to enable defender.</br> <img src="/resources/azure/defender/enable-defender-for-dns/step5.png"/>
