[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Identity / Password Requires Symbols

## Quick Info

| | |
|-|-|
| **Plugin Title** | Password Requires Symbols |
| **Cloud** | ORACLE |
| **Category** | Identity |
| **Description** | Ensures password policy requires at least one symbol. |
| **More Info** | A strong password policy enforces minimum length, expiration, reuse, and symbol usage. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Identity/Tasks/managingpasswordrules.htm |
| **Recommended Action** | Update the password policy to require the use of symbols. |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Identity" under the "Governance and Administration." </br> <img src="/resources/oracle/identity/password-requires-symbols/step2.png"/>
3. On the Identity menu, select the "Authentication" settings option.</br> <img src="/resources/oracle/identity/password-requires-symbols/step3.png"/>
4. On the "Authentication Settings" page, click on the "Edit" button to check "Password requires symbols" is enabled or not.</br> <img src="/resources/oracle/identity/password-requires-symbols/step4.png"/>
5. On the "Edit Authentication Settings" page, make sure "Password requires symbols" is enabled as per the best practices of Oracle cloud.</br> <img src="/resources/oracle/identity/password-requires-symbols/step5.png"/>
6. Repeat steps number 2 - 5 to check other Oracle cloud accounts.</br>
7. Navigate to "Identity" under the "Governance and Administration" and select the "Authentication" settings to set the "Password requires symbols".</br> <img src="/resources/oracle/identity/password-requires-symbols/step7.png"/>
8. Click on the "Edit" button to open the "Authentication" settings.</br> <img src="/resources/oracle/identity/password-requires-symbols/step8.png"/>
9. On the "Edit Authentication Settings" page, click on the checkbox next to the "Password requires symbols" and click on the "Save" button to make the changes.</br> <img src="/resources/oracle/identity/password-requires-symbols/step9.png"/>
10. Repeat steps number 7 - 9 to update the password policy to require the use of symbols. </br>
