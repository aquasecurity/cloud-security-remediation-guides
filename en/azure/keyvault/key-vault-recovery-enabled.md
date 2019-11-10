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
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "Key vault". </br> <img src="/resources/azure/keyvault/key-vault-recovery-enabled/step2.png"/>
3. Key Vault "Purge Protection and Soft Delete" feture cannot be checked or enable using the console. Need to use either PowerShell or Azure CLI to make the changes.</br> 
4. Paste the URL "https://docs.microsoft.com/en-us/cli/azure/authenticate-azure-cli?view=azure-cli-latest#code-try-0" and hit enter.</br> <img src="/resources/azure/keyvault/key-vault-recovery-enabled/step4.png"/>
5. Type the command "az login" to get into the Azure CLI.</br> <img src="/resources/azure/keyvault/key-vault-recovery-enabled/step5.png"/>
6. Visit the URL "https://microsoft.com/devicelogin" and enter the code shown in the Azure CLI.</br> 
7. Once you are into the "Azure CLI", check the screenshot accordingly.</br> <img src="/resources/azure/keyvault/key-vault-recovery-enabled/step7.png"/>
8. To verify that a key vault has soft-delete enabled, run the show command and look for the "Soft Delete Enabled?" attribute as shown in the screenshot.If the "Soft-Delete" and "Purge Protection" value is false then the "Soft Delete" as well as "Purge Protection" is not enabled.</br> <img src="/resources/azure/keyvault/key-vault-recovery-enabled/step8.png"/>
9. For enabling "Soft Delete" use the command as 'az keyvault show --name *vaultname* -o tsv | awk '{print $1}') --set properties.enableSoftDelete=true'." Make sure to replace *vaultname* to Key vault you are using.</br> <img src="/resources/azure/keyvault/key-vault-recovery-enabled/step9.png"/>
10. For enabling "Purge Protection" use the command as 'az resource update --id $(az keyvault show --name *vaultname* -o tsv | awk '{print $1}') --set properties.enablePurgeProtection=true'.Make sure to replace *vaultname* to Key vault you are using.</br> <img src="/resources/azure/keyvault/key-vault-recovery-enabled/step10.png"/>
11. Repeat steps number 2 - 10 to enable "Key Vault Recovery" option.</br>
