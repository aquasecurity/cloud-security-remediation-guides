[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / IAM / IAM Policies Present

## Quick Info

| | |
|-|-|
| **Plugin Title** | IAM Policies Present |
| **Cloud** | AWS |
| **Category** | IAM |
| **Description** | Ensure that required policies are present in all IAM roles. |
| **More Info** | Validate the presence of required policies in IAM roles in order to follow your organizations\'s security and compliance requirements. |
| **AWS Link** | https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html |
| **Recommended Action** | Modify IAM roles to attach required policies. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select "Services" and search for IAM.
    <img src="/resources/aws/iam/iam-policies-present/step1.png"/>
3. In the IAM dashboard, click on "Roles" from the left navigation panel.
       <img src="/resources/aws/iam/iam-policies-present/step2.png"/>
4. Select the role you want to modify to attach the required policy.
5. In the "Permissions" tab, click on "Attach policies" and select the required policies to meet security and compliance standards.
    <img src="/resources/aws/iam/iam-policies-present/step3.png"/>
6. Click "Attach policy" to finalize changes. Repeat for other roles as needed.