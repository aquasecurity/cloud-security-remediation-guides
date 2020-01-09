[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Key Vault / Key Expiration Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Key Expiration Enabled |
| **Cloud** | AZURE |
| **Category** | Key Vault |
| **Description** | Ensure that all Keys in Azure Key Vault have an expiry time set. |
| **More Info** | Setting an expiry time on all keys forces key rotation and removes unused and forgotten keys from being used. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/key-vault/about-keys-secrets-and-certificates |
| **Recommended Action** | 1. Go to Key vaults. 2. For each Key vault, click on Keys. 3. Ensure that each key in the vault has EXPIRATION DATE set as appropriate. |

## Detailed Remediation Steps
1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Key Vault . </br> <img src="/resources/azure/keyvault/key-expiration-enabled/step2.png"/>
3. On the "Key vault" page, select the "Key Vault" for which keys need to be verified.</br> <img src="/resources/azure/keyvault/key-expiration-enabled/step3.png"/>
4. On the "Key vaults-test-vault-azure" page, scroll down the left navigation panel and choose the "Keys" option.</br> <img src="/resources/azure/keyvault/key-expiration-enabled/step4.png"/>
5. On the "Key vaults-test-vault-azure - Keys" page, select the key and check for the "Expiration Date". If no "Expiration Date" is showing then the select "Key" do not have "Key Expiration Enabled."</br> <img src="/resources/azure/keyvault/key-expiration-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "Keys" in the "Key vaults."</br>
7. Navigate to the "Key vault", scroll down the left naviagtion panel and choose the "Keys" option.</br>  <img src="/resources/azure/keyvault/key-expiration-enabled/step7.png"/>
8. Select the "Key" which needs to have "Key Expiration Enabled" by clicking on the "Name" as a link option. </br>  <img src="/resources/azure/keyvault/key-expiration-enabled/step8.png"/>
9. On the "Key vaults - Keys" page click on the "Current Version" of the selected key.</br>  <img src="/resources/azure/keyvault/key-expiration-enabled/step9.png"/>
10. On the selected "key" page, click on the "Activation Date" and select the "Date and Time" accordingly. Select the "Set expiration date" and "Time" as per the requirements under the "Settings" tab.</br>  <img src="/resources/azure/keyvault/key-expiration-enabled/step10.png"/>
11. Click on the "Save" button at the top to make the changes.</br>  <img src="/resources/azure/keyvault/key-expiration-enabled/step11.png"/>
12. Repeat steps number 7 - 11 to enable "Key Expiration" for all the keys in the account.</br>
