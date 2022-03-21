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
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for SNS. </br> <img src="/resources/aws/sns/sns-topic-policies/step2.png"/>
3. In the left navigation panel, select Topics under SNS Dashboard. </br> <img src="/resources/aws/sns/sns-topic-policies/step3.png"/>
4. Select the Topic by clicking on the ID.</br> <img src="/resources/aws/sns/sns-topic-policies/step4.png"/>
5. In the Topic configuration page, scroll down and click on "Access policy" tab. </br> <img src="/resources/aws/sns/sns-topic-policies/step5.png"/>
6. Check the value of "Prinicipal" key. If it's set to (*) everyone then this topic allows access to everyone.</br> <img src="/resources/aws/sns/sns-topic-policies/step6.png"/>
7. To change the access policy, click on the "Edit" button at the top of the page. </br> <img src="/resources/aws/sns/sns-topic-policies/step7.png"/>
8. On the "Edit topic" page, scroll down to "Access policy" and in the "JSON editor" change the "Principal" key with the correct IAM role ARN eg. arn:aws:iam::066531304300:user/dev27. </br> <img src="/resources/aws/sns/sns-topic-policies/step8.png"/>
9. Click on "Save changes" button at the bottom of the page.</br> <img src="/resources/aws/sns/sns-topic-policies/step9.png"/>
10. Repeat steps 3-9 for all other SNS Topics across all regions.

