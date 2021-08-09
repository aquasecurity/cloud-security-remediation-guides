[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Group Inline Policies

## Quick Info

| | |
|-|-|
| **Plugin Title** | Group Inline Policies |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures that groups do not have any inline policies |
| **More Info** | Managed Policies are recommended over inline policies. |
| **AWS Link** | https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_managed-vs-inline.html |
| **Recommended Action** | Remove inline policies attached to groups |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for IAM. </br> <img src="/resources/aws/iam/iam-role-last-used/step2.png"/>
3. Scroll down the left navigation panel and choose "User groups". </br> <img src="/resources/aws/iam/iam-role-last-used/step3.png"/>
4. In the "User groups" page, click on the "Group name" to exapnd the respective attributes.</br> <img src="/resources/aws/iam/iam-role-last-used/step4.png"/>
5. In the "User groups" summary page, click on the "Permissions" and check for attached inline policies.</br> <img src="/resources/aws/iam/iam-role-last-used/step5.png"/>
6. Repeat steps 2 - 5 to check other "User groups" in the account.</br>
7. Navigate to IAM dashboard at https://console.aws.amazon.com/iam/.</br>
8. In the "IAM dashboard", click on the "User groups" option at the left navigation panel.</br>
9. In the "User groups" page, select the group name for which inline policies need to be removed.</br> <img src="/resources/aws/iam/iam-role-last-used/step9.png"/>
10. Select the inline policy by selecting the checkbox and click on the "Remove" button under the "Permissions" tab.</br> <img src="/resources/aws/iam/iam-role-last-used/step10.png"/>
11. On the "Remove" tab, enter the inline policy name and click on the "Delete" button to remove the inline policy.</br>  <img src="/resources/aws/iam/iam-role-last-used/step11.png"/>
12. Repeat steps number 7 - 11 to remove inline policies attached to groups.</br>

