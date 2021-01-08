[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Identity / Excessive Policies

## Quick Info

| | |
|-|-|
| **Plugin Title** | Excessive Policies |
| **Cloud** | ORACLE |
| **Category** | Identity |
| **Description** | Determine if there are an excessive number of policies in the account |
| **More Info** | Keeping the number of policies to a minimum helps reduce the chances of compromised accounts causing catastrophic damage to the account. Rather than creating new policies with the same statement for each group, common statements should be grouped under the same policy.  |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Identity/Concepts/policygetstarted.htm |
| **Recommended Action** | Limit the number of policies to prevent accidental authorizations |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Identity" under the "Governance and Administration." </br> <img src="/resources/oracle/identity/excessive-policies/step2.png"/>
3. On the Identity menu, select the "Policies" option.</br> <img src="/resources/oracle/identity/excessive-policies/step3.png"/>
4. On the "Policy" page select the policy by clicking on the "Name" as a link to check the "Policy Statement."</br> <img src="/resources/oracle/identity/excessive-policies/step4.png"/>
5. On the "Policy Statement" page, check whether we need the same "Policy" or not.</br> <img src="/resources/oracle/identity/excessive-policies/step5.png"/>
6. Repeat steps number 2 - 5 to check other "Policies" in the account.</br>
7. Navigate to "Identity" under the "Governance and Administration" and select the "Policies" settings to remove the "Excessive Policy".</br> <img src="/resources/oracle/identity/excessive-policies/step7.png"/>
8. On the "Policy" page, select the policy by clicking on the checkbox and click on "Delete" option at the top.</br> <img src="/resources/oracle/identity/excessive-policies/step8.png"/>
9. On the "Delete Policy" tab, click on the "Delete" button to make the changes.</br> <img src="/resources/oracle/identity/excessive-policies/step9.png"/>
10. Repeat steps number 7 - 9 to limit the number of policies to prevent accidental authorizations.</br>
