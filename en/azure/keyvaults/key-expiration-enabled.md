[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Key Vaults / Key Expiration Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Key Expiration Enabled |
| **Cloud** | AZURE |
| **Category** | Key Vaults |
| **Description** | Ensure that all Keys in Azure Key Vault have an expiry time set. |
| **More Info** | Setting an expiry time on all keys forces key rotation and removes unused and forgotten keys from being used. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/key-vault/about-keys-secrets-and-certificates |
| **Recommended Action** | Ensure each Key Vault has an expiry time set that provides for sufficient rotation. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. In the search bar at the top search for App Services. </br> <img src=“/resources/azure/appservice/.net-framework-version/step2.png”/>
3. Select the “App Services” by clicking on the “Name” link to access the configuration changes.</br> <img src=“/resources/azure/appservice/.net-framework-version/step3.png”/>
4. 


