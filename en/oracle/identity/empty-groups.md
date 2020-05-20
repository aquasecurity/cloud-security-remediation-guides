[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Identity / Empty Groups

## Quick Info

| | |
|-|-|
| **Plugin Title** | Empty Groups |
| **Cloud** | ORACLE |
| **Category** | Identity |
| **Description** | Ensures all groups have at least one member. |
| **More Info** | While having empty groups does not present a direct security risk, it does broaden the management landscape which could potentially introduce risks in the future. |
| **ORACLE Link** | https://docs.oracle.com/cd/E10391_01/doc.910/e10360/usergroups.htm |
| **Recommended Action** | Remove identity groups with no members. |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Identity" under the "Governance and Administration." </br> <img src="/resources/oracle/identity/empty-groups/step2.png"/>
3. On the Identity menu, select the "Groups" option.</br> <img src="/resources/oracle/identity/empty-groups/step3.png"/>
4. On the "Groups" page, select the "User group" by clicking on the "Name" as a link to access the group.</br> <img src="/resources/oracle/identity/empty-groups/step4.png"/>
5. On the selected group check that the group have at leat one member. If not then it's not as best practices recommended by Oracle.</br> <img src="/resources/oracle/identity/empty-groups/step5.png"/>
6. Repeat steps number 2 - 5 to check other groups in the account.</br>
7. Navigate to "Identity" under the "Governance and Administration" and select the "Groups" to delete the group one no users.</br> <img src="/resources/oracle/identity/empty-groups/step7.png"/>
8. Select the group with no users by clicking on the checkbox and click on the "Delete" option at the top to remove the selected group.</br> <img src="/resources/oracle/identity/empty-groups/step8.png"/>
9. On the "Delete group" tab, click on the "Delete" button to make the changes.</br> <img src="/resources/oracle/identity/empty-groups/step9.png"/>
10. Repeat steps number 7 - 9 to remove identity groups with no members.</br>

