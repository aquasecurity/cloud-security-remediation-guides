[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Key Vaults / Secret Expiration Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Secret Expiration Enabled |
| **Cloud** | AZURE |
| **Category** | Key Vaults |
| **Description** | Ensures that all secrets in Azure Key Vault have an expiry time set. |
| **More Info** | Setting an expiry time on all secrets forces secret rotation and removes unused and forgotten secrets from being used. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/secret-vault/about-secrets-secrets-and-certificates |
| **Recommended Action** | Ensure each Key Vault has an expiry time set that provides for sufficient rotation. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. In the search bar at the top search for Vaults and select "Key Vaults" from the search result. </br> <img src="/resources/azure/keyvault/secret-expiration-enabled/step2.png"/>
3. In the Key Vaults page, select a key vault by clicking on the “Name” link to access the configuration changes.</br> <img src="/resources/azure/keyvault/secret-expiration-enabled/step3.png"/>
4. Scroll down and click "Secrets" from the navigation pane on the left. </br> <img src="/resources/azure/keyvault/secret-expiration-enabled/step4.png"/>
5. Then, from the list of secrets, select a secret with no expiration date under "Expiration date" column.</br> <img src="/resources/azure/keyvault/secret-expiration-enabled/step5.png"/>
6. In the secret versions pane that opens, select the currently "Enabled" version by clicking on it.</br> <img src="/resources/azure/keyvault/secret-expiration-enabled/step6.png"/>
7. In the secret version pane, if the "Set expiration date" checkbox is not selected, then expiration is not set for this secret. This is a security vulnerability.</br> <img src="/resources/azure/keyvault/secret-expiration-enabled/step7.png"/>
8. Select the "Set expiration date" checkbox to enable expiration.</br> <img src="/resources/azure/keyvault/secret-expiration-enabled/step8.png"/>
9. Now click on the calendar for "Expiration date" and select a date after 27 days to set as expiration date.</br> <img src="/resources/azure/keyvault/secret-expiration-enabled/step9.png"/>
10. Finally, hit "Save" at the top of the pane to complete the changes.</br> <img src="/resources/azure/keyvault/secret-expiration-enabled/step10.png"/>
11. Repeat step number 3 - 10 for all other key vaults and keys without expiration date.
