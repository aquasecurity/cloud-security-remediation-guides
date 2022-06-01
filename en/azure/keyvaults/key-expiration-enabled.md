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
2. In the search bar at the top search for Vaults and select "Key Vaults" from the search result. </br> <img src="/resources/azure/keyvault/key-expiration-enabled/step2.png"/>
3. In the Key Vaults page select a key vault by clicking on the “Name” link to access the configuration changes.</br> <img src="/resources/azure/keyvault/key-expiration-enabled/step3.png"/>
4. From the list of keys, select key with no expiration date under "Expiration date" column.</br> <img src="/resources/azure/keyvault/key-expiration-enabled/step4.png"/>
5. In the key versions pane that opens, click "Rotation Policy" button at the top.</br> <img src="/resources/azure/keyvault/key-expiration-enabled/step5.png"/>
6. In the Rotation policy pane, click on the Expiry time textbox and enter 28. From the units dropdown next to the textbox, select "days".</br> <img src="/resources/azure/keyvault/key-expiration-enabled/step6.png"/>
7. Under the Rotation section, "Enable auto rotation" by selecting the "Enabled" radio button.</br> <img src="/resources/azure/keyvault/key-expiration-enabled/step7.png"/>
8. Select "Automatically renewat a given time after creation" for "Rotation option".
9. For "Rotation time" enter 18 and select "days" as the unit of time.
10. Finally, hit "Save" at the top of the pane to complete the changes.</br> <img src="/resources/azure/keyvault/key-expiration-enabled/step8.png"/>
11. Repeat steps 3 - 10 for all other key vaults and keys without expiration date.


