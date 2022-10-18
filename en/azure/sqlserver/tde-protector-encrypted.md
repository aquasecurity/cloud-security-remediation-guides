[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / SQL Server / TDE Protector Encrypted

## Quick Info

| | |
|-|-|
| **Plugin Title** | TDE Protector Encrypted |
| **Cloud** | AZURE |
| **Category** | SQL Server |
| **Description** | Ensures SQL Server TDE protector is encrypted with BYOK (Bring Your Own Key) |
| **More Info** | Enabling BYOK in the TDE protector allows for greater control and transparency, as well as increasing security by having full control of the encryption keys. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/sql-database/transparent-data-encryption-byok-azure-sql |
| **Recommended Action** | Ensure that a BYOK key is set for the Transparent Data Encryption of each SQL Server. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for "SQL servers". </br> <img src="/resources/azure/sqlserver/tde-protector-encrypted/step2.png"/>
3. On the "SQL server" page, select the SQL server that needs to be examined. </br> <img src="/resources/azure/sqlserver/tde-protector-encrypted/step3.png"/>
4. On the selected "SQL server" page, scroll down the left navigation panel and select "Transparent data encryption" under the "Security".</br> <img src="/resources/azure/sqlserver/tde-protector-encrypted/step4.png"/>
5. On the "Transparent data encryption" page, if "Transparent data encryption" is set to "Service-managed key" then the selected "SQL server TDE protector" is not encrypted with BYOK (Bring Your Own Key).</br> <img src="/resources/azure/sqlserver/tde-protector-encrypted/step5.png"/>
6. To ensure that a custom BYOK is used, select "Customer-managed key" for "Transparent data encryption".</br> <img src="/resources/azure/sqlserver/tde-protector-encrypted/step6.png"/>
7. Under "Key selection method" choose "Select a key" and click on "Change key" under "Key".</br> <img src="/resources/azure/sqlserver/tde-protector-encrypted/step7.png"/>
8. In the "Select a key" page, select the "Key vault" under "Key store type" and then select desired "Key" and "version" accordingly. Click on "Select" button at the bottom to proceed.</br> <img src="/resources/azure/sqlserver/tde-protector-encrypted/step8.png"/>
9. Click on the "Save" button at the top to make the necessary changes.</br> <img src="/resources/azure/sqlserver/tde-protector-encrypted/step9.png"/>
10. Reepat steps number 3 - 9 to ensure that a BYOK key is set for the Transparent Data Encryption of each SQL Server.</br>
