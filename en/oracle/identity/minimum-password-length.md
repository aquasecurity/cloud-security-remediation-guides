[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Identity / Minimum Password Length

## Quick Info

| | |
|-|-|
| **Plugin Title** | Minimum Password Length |
| **Cloud** | ORACLE |
| **Category** | Identity |
| **Description** | Ensures password policy requires a minimum password length. |
| **More Info** | A strong password policy enforces minimum length, expiration, reuse, and symbol usage. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Identity/Tasks/managingpasswordrules.htm |
| **Recommended Action** | Update the password policy to require a minimum password length. |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Identity" under the "Governance and Administration." </br> <img src="/resources/oracle/identity/minimum-password-length/step2.png"/>
3. On the Identity menu, select the "Authentication" settings option.</br> <img src="/resources/oracle/identity/minimum-password-length/step3.png"/>
4. On the "Authentication Settings" page, click on the "Edit" button to check "Minimum Password Length" is required or not.</br> <img src="/resources/oracle/identity/minimum-password-length/step4.png"/>
5. On the "Edit Authentication Settings" page, make sure "Minimum Password Length" is set above 8 characters as per the best practices of Oracle cloud.</br> <img src="/resources/oracle/identity/minimum-password-length/step5.png"/>
6. Repeat steps number 2 - 5 to check other Oracle cloud accounts.</br>
7. Navigate to "Identity" under the "Governance and Administration" and select the "Authentication" settings to set the "Minimum Password Length".</br> <img src="/resources/oracle/identity/minimum-password-length/step7.png"/>
8. Click on the "Edit" button to open the "Authentication" settings.</br> <img src="/resources/oracle/identity/minimum-password-length/step8.png"/>
9. On the "Edit Authentication Settings" page, enter the "Minimum Password Length" as 9 characters and click on the "Save" button to make the changes.</br> <img src="/resources/oracle/identity/minimum-password-length/step9.png"/>
10. Repeat steps number 7 - 9 to update the password policy to require a minimum password length. </br>
