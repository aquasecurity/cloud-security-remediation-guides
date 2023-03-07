[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Pub/Sub / Dead Lettering Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Dead Lettering Enabled |
| **Cloud** | GOOGLE |
| **Category** | Pub/Sub |
| **Description** | Ensure that each Google Pub/Sub subscription is configured to use dead-letter topic. |
| **More Info** | Enabling dead lettering will handle message failures by forwarding undelivered messages to a dead-letter topic that stores the message for later access. |
| **GOOGLE Link** | https://cloud.google.com/pubsub/docs/dead-letter-topics |
| **Recommended Action** | Ensure that dead letter topics are configured for all your Google Cloud Pub/Sub subscriptions. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose "Pub/Sub" to select the "Subscriptions" option.
3. Next to the subscription to update, selet <span>&#x22EE;</span> to open the "More Options" context menu.
4. In the context menu, select Edit.
5. In the Dead lettering section, select Enable dead lettering.
6. Choose or create a topic from the drop-down menu.
    - If the chosen topic does not have a subscription, the system prompts you to create one.
7. In the Maximum delivery attempts field, specify an integer between 5 and 100.
8. Click Update.
    - The details panel shows a list of possible action items. If any of the items show an error icon error, click the action item to resolve the issue.
9. Repeat steps 3 - 8 for any additional subscriptions requiring dead lettering to be enabled. 

**These configuration changes may incur additional costs**