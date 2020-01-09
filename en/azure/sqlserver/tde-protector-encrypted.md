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

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for SQL servers. </br> <img src="/resources/azure/sqlserver/tde-protector-encrypted/step2.png"/>
3. On the "SQL server" page, select the SQL server that needs to be examine. </br> <img src="/resources/azure/sqlserver/tde-protector-encrypted/step3.png"/>
4. On the selected "SQL server" page, scroll down the left navigation panel and select "Transparent data encryption" under the "Security" column.</br> <img src="/resources/azure/sqlserver/tde-protector-encrypted/step4.png"/>
5. On the "Transparent data encryption" page, if "Use your own key" is set to "NO" then the selected "SQL server TDE protector" is not encrypted with BYOK (Bring Your Own Key).</br> <img src="/resources/azure/sqlserver/tde-protector-encrypted/step5.png"/>
6. Repeat steps number 2 - 5 to verify other "SQL servers" in the account.</br>
7. Navigate to "SQL servers", on the "SQL servers" page select the "SQL server", scroll down the left navigation panel and choose "Transparent data encryption" under the "Security."</br> <img src="/resources/azure/sqlserver/tde-protector-encrypted/step7.png"/>
8. On the "Transparent data encryption" page, click on the "Yes" button next to the "Use your own key". Select the "Key vault" and "Key" accordingly. Click on the checkbox next to "Make the selected key the default TDE protector."</br> <img src="/resources/azure/sqlserver/tde-protector-encrypted/step8.png"/>
9. Click on the "Save" button at the top to make the changes.</br> <img src="/resources/azure/sqlserver/tde-protector-encrypted/step9.png"/>
10. Reepat steps number 7 - 9 to ensure that a BYOK key is set for the Transparent Data Encryption of each SQL Server.</br>
