[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Active Directory / Monitor External Accounts with Write Permissions

## Quick Info

| | |
|-|-|
| **Plugin Title** | Monitor External Accounts with Write Permissions |
| **Cloud** | AZURE |
| **Category** | Security Center |
| **Description** | Ensures that External Accounts with Write Permissions are being Monitored in Security Center |
| **More Info** | External Accounts with Write Permissions should be monitored to meet you organization's security compliance requirements. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/security-center/security-center-policy-definitions |
| **Recommended Action** | Enable Monitor for External Accounts with Write Permissions by ensuring AuditIfNotExists setting is used for 'External accounts with write permissions should be removed from your subscription' from the Azure Security Center. |

## Detailed Remediation Steps

1. ASC Default policies should monitor for this by default. If no ASC Default policy found, this policy can be manually assigned and enabled. 
2. Log into the Microsoft Azure Management Console.
3. Select the "Search resources, services, and docs" option at the top and search for Resource Groups.
4. Select the corresponding resource group by clicking on the 'name' link.
5. On the navigation pane to the left, select "Policies" in the Settings section.
6. In the policies section, select "Assign Policy" at the top of the section menu.
7. Assign the scope this policy should cover and any necessary exclusions.
8. In the Policy Definition section, select "External accounts with write permissions should be removed from your subscription".
9. Ensure that Policy Enforcement is set to 'enabled' and then select Next. 
10. In the Parameters section, set the Effect to 'AuditIfNotExists'.
11. Optional - Assign Remediation and Non-Compliance Messages.
12. Review and Create the policy.

