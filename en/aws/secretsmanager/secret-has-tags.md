[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Secrets Manager / Secret Manager Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | Secret Manager Has Tags |
| **Cloud** | AWS |
| **Category** | Secrets Manager |
| **Description** | Ensure that Secrets have tags. |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/secretsmanager/latest/userguide/managing-secrets_tagging.html |
| **Recommended Action** | Update Secrets and add tags. |

## Detailed Remediation Steps

1. Log into the AWS Management Console.
2. Select the "Services" option and search for Secrets Manager. </br> <img src="/resources/aws/secretsmanager/secret-has-tags/step2.png"/>
3. Click on "Secrets" from navigation panel on the left.</br> <img src="/resources/aws/secretsmanager/secret-has-tags/step3.png"/>
4. Select the secret which needs to have tags by Clicking on the secret name.</br> <img src="/resources/aws/secretsmanager/secret-has-tags/step4.png"/></br> <img src="/resources/aws/secretsmanager/secret-has-tags/step5.png"/><img src="/resources/"/>
6. Enter the key value pair for the tag and Click save.</br> <img src="/resources/aws/secretsmanager/secret-has-tags/step6.png"/>


