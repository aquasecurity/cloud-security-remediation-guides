[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Key Vault / Key Vault Recovery Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Key Vault Recovery Enabled |
| **Cloud** | AZURE |
| **Category** | Key Vault |
| **Description** | Ensures that Purge Protection and Soft Delete are enabled on all Key Vaults. |
| **More Info** | Purge Protection and Soft Delete are features that safeguard losing key access. With these setting enabled, key vaults have recovery actions available to restore deleted or compromised key vaults. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/key-vault/key-vault-ovw-soft-delete |
| **Recommended Action** | 1. Login to the Azure CLI. 2. Use the command and change *vaultname* to the vault to enable Soft Delete: 'az resource update --id $(az keyvault show --name *vaultname* -o tsv | awk '{print $1}') --set properties.enableSoftDelete=true'. 3. Use the command and change *vaultname* to the vault to enable Surge Protection: 'az resource update --id $(az keyvault show --name *vaultname* -o tsv | awk '{print $1}') --set properties.enablePurgeProtection=true' |

## Detailed Remediation Steps

