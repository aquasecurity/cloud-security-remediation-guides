[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Pub/Sub / Topic Labels Added

## Quick Info

| | |
|-|-|
| **Plugin Title** | Topic Labels Added |
| **Cloud** | GOOGLE |
| **Category** | Pub/Sub |
| **Description** | Ensure that all Pub/Sub topics have labels added. |
| **More Info** | Labels are a lightweight way to group resources together that are related to or associated with each other. It is a best practice to label cloud resources to better organize and gain visibility into their usage. |
| **GOOGLE Link** | https://cloud.google.com/pubsub/docs/labels |
| **Recommended Action** | Ensure labels are added to all Pub/Sub topics. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose "Pub/Sub" to select the "Topics" option. </br> <img src="/resources/google/pubsub/topic-labels-added/step2.png">
3. On the "Topics" page, select the topic which needs to be verified whether it has labels added or not by clicking on the checkbox next to its name.</br> <img src="/resources/google/pubsub/topic-labels-added/step3.png"/>
4. From the panel on the right side, select "Labels" and check if there are any labels shown. If not, the topic does not have labels added.</br> <img src="/resources/google/pubsub/topic-labels-added/step4.png"/>
5. Repeat steps number 3-4 to check other topics in the project.</br>
6. Navigate to "Pub/Sub", choose "Topics". From the panel on the right side, click on "Labels" and then click on the checkbox next to the name of the "Topic" which needs to have labels added.</br> <img src="/resources/google/pubsub/topic-labels-added/step4.png"/>
7. Click on "Add Label", and add key and value for the label. Add as many labels as you want and then click "Save".</br> <img src="/resources/google/pubsub/topic-labels-added/step7.png"/>
8. Repeat steps number 7-8 to add labels to all other topics in the project.</br>