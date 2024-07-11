# AWS / EventBridge / Event Bus Public Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Event Bus Public Access |
| **Cloud** | AWS |
| **Category** | EventBridge |
| **Description** | Ensure that EventBridge event bus is configured to prevent exposure to public access. |
| **More Info** | The default event bus in your Amazon account only allows events from one account. You can grant additional permissions to an event bus by attaching a resource-based policy to it. |
| **AWS Link** | https://docs.amazonaws.cn/en_us/eventbridge/latest/userguide/eb-event-bus-perms.html |
| **Recommended Action** | Configure EventBridge event bus policies that allow access to whitelisted/trusted account principals but not public access. |

## Detailed Remediation Steps

1. From the AWS management console, select Amazon EventBridge and click on Dashboard. </br> <img src="/resources/aws/eventbridge/step1.png"/>
2. Click on the event bus which contains the offending policy. </br> <img src="/resources/aws/eventbridge/step2.png"/>
3. Select Permissions and click on Manage permissions. </br> <img src="/resources/aws/eventbridge/step3.png"/>
4. Edit the Resource-based policy to allow access to whitelisted/trusted account principals but not public access.</br> <img src="/resources/aws/eventbridge/step4.png"/>