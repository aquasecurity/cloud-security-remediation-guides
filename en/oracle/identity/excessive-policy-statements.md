[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Identity / Excessive Policy Statements

## Quick Info

| | |
|-|-|
| **Plugin Title** | Excessive Policy Statements |
| **Cloud** | ORACLE |
| **Category** | Identity |
| **Description** | Determine if there are an excessive number of policy statements in the account |
| **More Info** | Keeping the number of policy statements to a minimum helps reduce the chances of compromised accounts causing catastrophic damage to the account. Common statements should be grouped under the same policy.  |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Identity/Concepts/policygetstarted.htm |
| **Recommended Action** | Limit the number of policy statements to prevent accidental authorizations |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Identity" under the "Governance and Administration." </br> <img src="/resources/oracle/identity/excessive-policy-statements/step2.png"/>
3. On the Identity menu, select the "Policies" option.</br> <img src="/resources/oracle/identity/excessive-policy-statements/step3.png"/>
4. On the "Policy" page select the policy by clicking on the "Name" as a link to check the "Policy Statement."</br> <img src="/resources/oracle/identity/excessive-policy-statements/step4.png"/>
5. On the "Policy Statement" page, check whether we need all the same "Policy Statement" or not or if there is any duplicacy in the policy statement.</br> <img src="/resources/oracle/identity/excessive-policy-statements/step5.png"/>
6. Repeat steps number 2 - 5 to check other "Policies" in the account.</br>
7. Navigate to "Identity" under the "Governance and Administration" and select the "Policies" settings to remove the "Excessive Policy Statements".</br> <img src="/resources/oracle/identity/excessive-policy-statements/step7.png"/>
8. On the "Policy" page, access the policy by clicking on the "Name" as a link.</br> <img src="/resources/oracle/identity/excessive-policy-statements/step8.png"/>
9. On the "Policy Statement" page, click on the "Edit Policy Statements" button to remove the excessive policy statements.</br> <img src="/resources/oracle/identity/excessive-policy-statements/step9.png"/>
10. On the "Edit Policy Statements" page, click on the remove icon at the extreme right of the policy statement to remove the selected statement. <img src="/resources/oracle/identity/excessive-policy-statements/step10.png"/>
11. Click on the "Save Changes" button at the bottom to make the changes.</br> <img src="/resources/oracle/identity/excessive-policy-statements/step11.png"/>
12. Repeat steps number 7 - 11 to limit the number of policy statements to prevent accidental authorizations.</br>

