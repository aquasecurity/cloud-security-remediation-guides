[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / DynamoDB / DynamoDB Table Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | DynamoDB Table Has Tags |
| **Cloud** | AWS |
| **Category** | DynamoDB |
| **Description** | Ensure that DynamoDB tables have tags |
| **More Info** |Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage.  |
| **AWS Link** | https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Tagging.html |
| **Recommended Action** | Modify dynamoDB table and add tags |

## Detailed Remediation Steps 

1. Log into the AWS Management Console.
2. Select the "Services" option and search for "DynamoDB" and Click on "DynamoDB".</br> <img src="/resources/aws/dynamodb/default-security-group/step2.png"/>
3. On "DynamoDB Dashboard" page Click on "Tables" from left navigation panel.</br> <img src="/resources/aws/dynamodb/dynamodb-table-has-tags/step3.png"/>
4. On dynamodb tables list page Click on the table Name which needs to have tags.</br> <img src="/resources/aws/dynamodb/dynamodb-table-has-tags/step4.png"/>
5. On Table details page choose "Additional Settings" tab from navigation panel on the top.</br> <img src="/resources/aws/dynamodb/dynamodb-table-has-tags/step5.png"/>
6. Under "Additional Settings" tab scroll down to "Tags" section. Click on "Manage Tags" button to manage new tags.</br> <img src="/resources/aws/dynamodb/dynamodb-table-has-tags/step6.png"/>
7. On "Manage Tags" page click on "Add new tags" button and enter key-value for the tag and Click on "Save Changes" button.</br> <img src="/resources/aws/dynamodb/dynamodb-table-has-tags/step7.png"/> 



