[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ACM / ACM Certificate Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | ACM Certificate Has Tags |
| **Cloud** | AWS |
| **Category** | ACM |
| **Description** | Ensure that ACM Certificates have tags |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage |
| **AWS Link** | https://docs.aws.amazon.com/acm/latest/userguide/tags.html |
| **Recommended Action** | Modify ACM certificate and add tags |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "ACM" and Click on "Amazon Certificate Manager".</br> <img src="/resources/aws/acm/acm-certificate-has-tags/step2.png"/>
3. On "Amazon Certificate Manager" page Click on "list certificates" from left navigation panel.</br> <img src="/resources/aws/acm/acm-certificate-has-tags/step3.png"/>
4. On ACM certificate list page Click on the certificate Name which needs to have tags.</br> <img src="/resources/aws/acm/acm-certificate-has-tags/step4.png"/>
5. On certificate details page scroll down to "Tags" section and Click on "Manage Tags" button.</br> <img src="/resources/aws/acm/acm-certificate-has-tags/step5.png"/>
6. On "Manage Tags" page Click on "Add Tag" button enter the Key value of tag and Click "Submit" button.</br> <img src="/resources/aws/acm/acm-certificate-has-tags/step6.png"/>
