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
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for IAM. </br><img src="/resources/aws/iam/empty-groups/step2.png"/>
3. Scroll down the left navigation panel and choose "User Groups" under "Access management". </br><img src="/resources/aws/iam/empty-groups/step3.png"/>
4. Under the "User Groups" configuration panel check the "Users" column. If the "Users" column won't have any user make sure to delete that "Group" as it can potentially increase risks in the future. Select the "Groups" with no user.</br><img src="/resources/aws/iam/empty-groups/step4.png"/>
5. Click on the "Delete" button at the top right to delete the selected "User Groups".</br><img src="/resources/aws/iam/empty-groups/step5.png"/>
6. In the "Delete User groups" pop up type "delete" in the text box and click "Delete" button to delete the selected "Group".</br><img src="/resources/aws/iam/empty-groups/step6.png"/>
7. Repeat steps number 3 and 6 to verify other "Groups" with at least one user.</br>
