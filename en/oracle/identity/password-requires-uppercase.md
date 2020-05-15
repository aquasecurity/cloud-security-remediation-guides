[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Identity / Password Requires Uppercase

## Quick Info

| | |
|-|-|
| **Plugin Title** | Password Requires Uppercase |
| **Cloud** | ORACLE |
| **Category** | Identity |
| **Description** | Ensures password policy requires at least one uppercase character. |
| **More Info** | A strong password policy enforces minimum length, expirations, reuse, and symbol usage. |
| **ORACLE Link** | https://docs.oracle.com/cd/E17904_01/admin.1111/e10029/pwdpolicies.htm#OIDAG2472 |
| **Recommended Action** | Update the password policy to require the use of uppercase characters. |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Identity" under the "Governance and Administration." </br> <img src="/resources/oracle/identity/password-requires-uppercase/step2.png"/>
3. On the Identity menu, select the "Authentication" settings option.</br> <img src="/resources/oracle/identity/password-requires-uppercase/step3.png"/>
4. On the "Authentication Settings" page, click on the "Edit" button to check "Password requires uppercase" is enabled or not.</br> <img src="/resources/oracle/identity/password-requires-uppercase/step4.png"/>
5. On the "Edit Authentication Settings" page, make sure "Password requires uppercase" is enabled as per the best practices of Oracle cloud.</br> <img src="/resources/oracle/identity/password-requires-uppercase/step5.png"/>
6. Repeat steps number 2 - 5 to check other Oracle cloud accounts.</br>
7. Navigate to "Identity" under the "Governance and Administration" and select the "Authentication" settings to set the "Password requires uppercase".</br> <img src="/resources/oracle/identity/password-requires-uppercase/step7.png"/>
8. Click on the "Edit" button to open the "Authentication" settings.</br> <img src="/resources/oracle/identity/password-requires-uppercase/step8.png"/>
9. On the "Edit Authentication Settings" page, click on the checkbox next to the "Password requires uppercase" and click on the "Save" button to make the changes.</br> <img src="/resources/oracle/identity/password-requires-uppercase/step9.png"/>
10. Repeat steps number 7 - 9 to update the password policy to require the use of uppercase characters. </br>
