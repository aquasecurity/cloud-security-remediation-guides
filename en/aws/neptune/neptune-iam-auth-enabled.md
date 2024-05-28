[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Neptune / Neptune Database IAM Authentication Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Neptune Database IAM Authentication Enabled |
| **Cloud** | AWS |
| **Category** | Neptune |
| **Description** | Ensure that AWS Neptune database instance has IAM database authentication feature enabled. |
| **More Info** | Enabling IAM authentication for AWS Neptune adds an extra layer of security by allowing access control through IAM credentials. It ensures that network traffic for clusters is encrypted using SSL and allows centralized management. All authentication requests are automatically signed with a secure access key instead of using a password. |
| **AWS Link** | https://docs.aws.amazon.com/neptune/latest/userguide/iam-auth.html |
| **Recommended Action** | Modify Neptune database instance and enable IAM database authentication. |

## Detailed Remediation Steps 
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "Neptune".</br> <img src="/resources/aws/neptune/neptune-iam-auth-enabled/step2.png"/>
3. On "Neptune Dashboard" page, Click on "Clusters" from left navigation panel.</br> <img src="/resources/aws/neptune/neptune-iam-auth-enabled/step3.png"/>
4. On Neptune clusters list page, Click on the cluster name on which you need to enable IAM authentication.</br> <img src="/resources/aws/neptune/neptune-iam-auth-enabled/step4.png"/>
5. On Cluster details page, click on "Modify" button.</br> <img src="/resources/aws/neptune/neptune-iam-auth-enabled/step5.png"/>
6. Scroll down on "Modify Cluster" page and under "Additional settings" section, select "Turn on IAM Authentication" checkbox and click on "Next" button.</br> <img src="/resources/aws/neptune/neptune-iam-auth-enabled/step6.png"/>
7. Under "Scheduling of modifications" section check "Apply immediately" checkbox and, Click on "Submit" button.</br> <img src="/resources/aws/neptune/neptune-iam-auth-enabled/step7.png"/> 
