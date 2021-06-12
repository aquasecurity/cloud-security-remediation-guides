[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / IAM Role Last Used

## Quick Info

| | |
|-|-|
| **Plugin Title** | IAM Role Last Used |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures IAM roles that have not been used within the given time frame are deleted. |
| **More Info** | IAM roles that have not been used for a long period may contain old access policies that could allow unintended access to resources if accidentally attached to new services. These roles should be deleted. |
| **AWS Link** | https://aws.amazon.com/about-aws/whats-new/2019/11/identify-unused-iam-roles-easily-and-remove-them-confidently-by-using-the-last-used-timestamp/ |
| **Recommended Action** | Delete IAM roles that have not been used within the expected time frame. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for IAM. </br> <img src="/resources/aws/iam/iam-role-last-used/step2.png"/>
3. Scroll down the left navigation panel and choose "Roles". </br><img src="/resources/aws/iam/iam-role-last-used/step3.png"/>
4. On the "Roles" page, scroll down and check the "Last Activity" column to verify when the IAM Roles are last used.</br> <img src="/resources/aws/iam/iam-role-last-used/step4.png"/>
5. For any Roles with the attribute "None" in the "Last Activity", click on the Role and check the Creation time.</br> <img src="/resources/aws/iam/iam-role-last-used/step5.png"/>
6. Repeat steps 2 - 4 to verify IAM Roles in other AWS account.</br>
7. Navigate to IAM dashboard at https://console.aws.amazon.com/iam/.</br>
8. In the "IAM dashboard", click on the "Roles" option at the left navigation panel.</br> <img src="/resources/aws/iam/iam-role-last-used/step8.png"/>
9. Select the roles whose "Last Activity" is greater then 90 days or whose Creation time is greater then 90 days but showing None in Last Activity.</br> <img src="/resources/aws/iam/iam-role-last-used/step9.png"/>
10. Click on the "Delete" option at the top to remove the selected IAM roles.</br> <img src="/resources/aws/iam/iam-role-last-used/step10.png"/>
11. On the "Delete role" tab, click on the "Yes, delete" button to make the changes.</br> <img src="/resources/aws/iam/iam-role-last-used/step11.png"/>
12. Repeat steps number 7 - 11 to delete IAM roles that have not been used within the expected time frame. </br>



