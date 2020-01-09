[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / DNS / DNS Security Signing Algorithm

## Quick Info

| | |
|-|-|
| **Plugin Title** | DNS Security Signing Algorithm |
| **Cloud** | GOOGLE |
| **Category** | DNS |
| **Description** | Ensures that DNS Security is not using the RSASHA1 algorithm for key or zone signing |
| **More Info** | DNS Security is a feature that authenticates all responses to domain name lookups. This prevents attackers from committing DNS hijacking or man in the middle attacks. |
| **GOOGLE Link** | https://cloud.google.com/dns/docs/dnssec |
| **Recommended Action** | Ensure that all managed zones using DNSSEC are not using the RSASHA1 algorithm for key or zone signing. |

## Detailed Remediation Steps

