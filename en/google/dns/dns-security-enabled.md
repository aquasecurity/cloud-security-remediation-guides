[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / DNS / DNS Security Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | DNS Security Enabled |
| **Cloud** | GOOGLE |
| **Category** | DNS |
| **Description** | Ensures that DNS Security is enabled on all managed zones |
| **More Info** | DNS Security is a feature that authenticates all responses to domain name lookups. This prevents attackers from committing DNS hijacking or man in the middle attacks. |
| **GOOGLE Link** | https://cloud.google.com/dns/docs/dnssec |
| **Recommended Action** | Ensure DNSSEC is enabled for all managed zones in the cloud DNS service. |

## Detailed Remediation Steps
1. Log in to the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Network Services" option under the "NETWORKING" and select the "Cloud DNS." </br> <img src="/resources/google/dns/dns-security-enabled/step2.png"/>
3. On the "Cloud DNS" page, select the "Zone name" which needs to be checked for the "DNS Security."</br> <img src="/resources/google/dns/dns-security-enabled/step3.png"/>
4. On the selected "Zone" check the "DNSSEC" is showing "Off" or "ON". If it's turned off then it cannot authenticates all responses to domain name lookups.</br> <img src="/resources/google/dns/dns-security-enabled/step4.png"/>
5. Repeat steps number 2 - 4 to check other DNS in the account.</br>
6. Navigate to the "Load balancing" option under the "Netowrk Services" of the "NETWORKING", choose the "Cloud DNS" option and select the "DNS".</br> <img src="/resources/google/dns/dns-security-enabled/step6.png"/>
7. On the "Cloud DNS" place, select the "Zone" and click on the dropdown menu below the "DNSSEC."</br> <img src="/resources/google/dns/dns-security-enabled/step7.png"/>
8. On the selected "Cloud DNS", select the "ON" from the dropdown menu of "DNSSEC."</br> <img src="/resources/google/dns/dns-security-enabled/step8.png"/>
9. On the "Enabling DNSSEC" tab, click on the "Enable" button to make the changes.</br> <img src="/resources/google/dns/dns-security-enabled/step9.png"/>
10. Repeat steps number 6 - 9 to ensure "DNSSEC" is enabled for all managed zones in the cloud DNS service.</br>
