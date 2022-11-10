[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Key Vaults / Key Vault Recovery Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Key Vault Recovery Enabled |
| **Cloud** | AZURE |
| **Category** | Key Vaults |
| **Description** | Ensures that Purge Protection and Soft Delete are enabled on all Key Vaults |
| **More Info** | Purge Protection and Soft Delete are features that safeguard losing key access. With these setting enabled, key vaults have recovery actions available to restore deleted or compromised key vaults. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/key-vault/key-vault-ovw-soft-delete |
| **Recommended Action** | Once Key Vaults are created, the Azure CLI must be used to update the vault Soft Delete and Purge Protection settings. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. In the search bar at the top search for Vaults and select "Key Vaults" from the search result. </br> <img src="/resources/azure/keyvault/key-vault-recovery-enabled/step2.png"/>
3. In the Key Vaults page select a key vault by clicking on the "Name" link to access the configuration changes.</br> <img src="/resources/azure/keyvault/key-vault-recovery-enabled/step3.png"/>
4. Scroll down and click "Properties" from the navigation pane on the left. </br> <img src="/resources/azure/keyvault/key-vault-recovery-enabled/step4.png"/>
5. If under "Soft delete" the "Disable purge protection" radio button is selected, then vaults and objects can be deleted with no recovery possible. This is against the best practices.</br> <img src="/resources/azure/keyvault/key-vault-recovery-enabled/step5.png"/>
6. Select the "Enable purge protection" radio button to allow only soft deletes so that vaults and objects can be recovered if needed.</br> <img src="/resources/azure/keyvault/key-vault-recovery-enabled/step6.png"/>
7. Finally, hit "Save" at the top of the pane to complete the changes.</br> <img src="/resources/azure/keyvault/key-vault-recovery-enabled/step7.png"/>
11. Repeat step number 3 - 7 for all other key vaults.

