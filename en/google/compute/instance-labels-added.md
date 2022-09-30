[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Instance Labels Added

## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance Labels Added |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensure that all Virtual Machine instances have labels added. |
| **More Info** | Labels are a lightweight way to group resources together that are related to or associated with each other. It is a best practice to label cloud resources to better organize and gain visibility into their usage.Labels are a lightweight way to group resources together that are related to or associated with each other. It is a best practice to label cloud resources to better organize and gain visibility into their usage. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/labeling-resources |
| **Recommended Action** | Ensure labels are added to all VM instances. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Compute Engine" to select the "VM Instances" option. </br> <img src="/resources/google/compute/instance-labels-added/step2.png"/>
3. On the "Instances" page, select the instance which needs to be verified whether it has labels added or not by clicking on the checkbox next to its name.</br> <img src="/resources/google/compute/instance-labels-added/step3.png"/>
4. From the panel on the right side, select "Labels" and check if there are any labels shown. If not, the VM Instance does not have labels added.</br> <img src="/resources/google/compute/instance-labels-added/step4.png"/>
5. Repeat steps number 3-4 to check other instances in the project.</br>
6. Navigate to "Compute Engine", choose "VM Instances". From the panel on the right side, click on "Labels" and then click on the checkbox next to the name of the "Instance" which needs to have labels added.</br> <img src="/resources/google/compute/instance-labels-added/step4.png"/>
7. Click on "Add Label" and add key and value for the label. Add as many labels as you want and then click "Save".</br> <img src="/resources/google/compute/instance-labels-added/step7.png"/>
8. Repeat steps number 7-8 to add labels to all other instances in the project.</br>
