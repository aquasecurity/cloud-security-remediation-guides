[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Application Gateway / Application Gateway WAF Prevention Mode Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Application Gateway WAF Prevention Mode Enabled |
| **Cloud** | AZURE |
| **Category** | Application Gateway |
| **Description** | Ensure that WAF policy for Microsoft Azure Application gateway is set to Prevention mode |
| **More Info** | Azure Web Application Firewall (WAF) on Azure Application Gateway provides centralized protection of your web applications from common exploits and vulnerabilities. Web applications are increasingly targeted by malicious attacks that exploit commonly known vulnerabilities. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/web-application-firewall/ag/ag-overview |
| **Recommended Action** | Modify application gateway WAF policy and enable prevention mode. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Application Gateway. </br> <img src="/resources/azure/applicationGateway/ap-waf-prevention-mode/step2.png"/>
3. Select the "Application Gateway" by clicking the "Name" as a link to get into the configuration changes. </br> <img src="/resources/azure/applicationGateway/ap-waf-prevention-mode/step3.png"/>
4. On "Virtual machine" navigation panel and choose "Web Application Firewall" under settings. </br> <img src="/resources/azure/applicationGateway/ap-waf-prevention-mode/step4.png"/>
5. On WAF page set WAF status to enabled and WAF Mode to "Prevention" and Click save from top navigation bar. </br> <img src="/resources/azure/applicationGateway/ap-waf-prevention-mode/step5.png"/>