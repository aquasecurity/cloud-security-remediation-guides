[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Identity / Users MFA Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Users MFA Enabled |
| **Cloud** | ORACLE |
| **Category** | Identity |
| **Description** | Ensures a multi-factor authentication device is enabled for all users within the account. |
| **More Info** | User accounts should have an MFA device setup to enable two-factor authentication. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Identity/Tasks/usingmfa.htm |
| **Recommended Action** | Enable an MFA device for the user account. |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Identity" under the "Governance and Administration." </br> <img src="/resources/oracle/identity/users-mfa-enabled/step2.png"/>
3. On the Identity menu, select the "Users" option.</br> <img src="/resources/oracle/identity/users-mfa-enabled/step3.png"/>
4. On the "Users" page, select the "User" and click on the "Name" as a link to access the user settings.</br> <img src="/resources/oracle/identity/users-mfa-enabled/step4.png"/>
5. On the selected user, check if it's showing to "Enable Multi-Factor Authentication".</br> <img src="/resources/oracle/identity/users-mfa-enabled/step5.png"/>
6. Repeat steps number 2 - 5 to check other users in the account.</br>
7. Navigate to "Identity" under the "Governance and Administration", click on the "Users" settings to enable the "MFA" and select the user on which changes needs to be done.</br> <img src="/resources/oracle/identity/users-mfa-enabled/step7.png"/>
8. On the selected user click on the "Enable Multi-Factor Enable Authentication" option at the top.</br> <img src="/resources/oracle/identity/users-mfa-enabled/step8.png"/>
9. Follow the next steps as mentioned in "Enable Multi-Factor Enable Authentication" tab and enter the "Verfication code" obtain on your "Authenticator" application and click on the "Verify" button.</br> <img src="/resources/oracle/identity/users-mfa-enabled/step9.png"/>
10. Repeat steps number 7 - 9 to enable an MFA device for the user account.</br>


