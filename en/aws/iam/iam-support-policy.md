[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / IAM Support Policy

## Quick Info

| | |
|-|-|
| **Plugin Title** | IAM Support Policy |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensures that an IAM role, group or user exists with specific permissions to access support center. |
| **More Info** | AWS provides a support center that can be used for incident notification and response, as well as technical support and customer services. An IAM Role should be present to allow authorized users to manage incidents with AWS Support. |
| **AWS Link** | https://docs.aws.amazon.com/awssupport/latest/user/accessing-support.html |
| **Recommended Action** | Ensure that an IAM role has permission to access support center. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select "Services" and search for IAM.
        <img src="/resources/aws/iam/iam-support-policy/step1.png"/>
3. In the IAM dashboard, click on "Roles" from the left navigation panel.
        <img src="/resources/aws/iam/iam-support-policy/step2.png"/>
4. Select the role you want to modify to allow access to the AWS Support Center.
5. In the "Permissions" tab, click on "Attach policies".
6. Search for and attach the "AWSSupportAccess" policy to enable access to support features.
        <img src="/resources/aws/iam/iam-support-policy/step3.png"/>
7. Click "Attach policy" to apply changes. Repeat for other roles, groups, or users as needed.