[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / Empty Groups

## Quick Info

| | |
|-|-|
| **Plugin Title** | Empty Groups |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures all groups have at least one member |
| **More Info** | While having empty groups does not present a direct security risk, it does broaden the management landscape which could potentially introduce risks in the future. |
| **AWS Link** | http://docs.aws.amazon.com/IAM/latest/UserGuide/Using_WorkingWithGroupsAndUsers.html |
| **Recommended Action** | Remove unused groups without users |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for IAM. </br><img src="/resources/aws/iam/empty-groups/step2.png"/>
3. Scroll down the left navigation panel and choose "Groups". </br><img src="/resources/aws/iam/empty-groups/step3.png"/>
4. Under the "Groups" configuration panel check the "Users" column.If the "Users" column won't have any user make sure to delete that "Group" as it could potentially introduce risks in the future. </br><img src="/resources/aws/iam/empty-groups/step4.png"/>
5. Repeat steps number 3 and 4 to verify other "Groups" with at least one user.</br>
6. Click on the "Groups" in the left navigation panel and select the "Group" with no user.</br><img src="/resources/aws/iam/empty-groups/step6.png"/>
7. Select "Group Actions" option from the top menu and click on the "Delete Group" to delete the selected "Group".</br><img src="/resources/aws/iam/empty-groups/step7.png"/>
8. Click on the "Yes,Delete" button in the "Delete Group" tab to delete the selected "Group".</br><img src="/resources/aws/iam/empty-groups/step8.png"/>
