[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / SNS / SNS Topic Policies

## Quick Info

| | |
|-|-|
| **Plugin Title** | SNS Topic Policies |
| **Cloud** | AWS |
| **Category** | SNS |
| **Description** | Ensures SNS topics do not allow global send or subscribe. |
| **More Info** | SNS policies should not be configured to allow any AWS user to subscribe or send messages. This could result in data leakage or financial DDoS. |
| **AWS Link** | http://docs.aws.amazon.com/sns/latest/dg/AccessPolicyLanguage.html |
| **Recommended Action** | Adjust the topic policy to only allow authorized AWS users in known accounts to subscribe. |

## Detailed Remediation Steps

