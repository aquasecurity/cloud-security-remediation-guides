[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / DNS / DNS Zone Labels Added

## Quick Info

| | |
|-|-|
| **Plugin Title** | DNS Zone Labels Added |
| **Cloud** | GOOGLE |
| **Category** | DNS |
| **Description** | Ensure Cloud DNS zones have labels added. |
| **More Info** | Labels are a lightweight way to group resources together that are related to or associated with each other. It is a best practice to label cloud resources to better organize and gain visibility into their usage.Labels are a lightweight way to group resources together that are related to or associated with each other. It is a best practice to label cloud resources to better organize and gain visibility into their usage. |
| **GOOGLE Link** | https://cloud.google.com/dns/docs/zones |
| **Recommended Action** | Ensure labels are added for all managed zones in the cloud DNS service. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose "Network Services" to select the "Cloud DNS" option. </br> <img src="/resources/google/dns/dns-zone-labels-added/step2.png">
3. On the "Cloud DNS" page, select the DNS Zone which needs to be verified whether it has labels added or not by clicking on the checkbox next to its name.</br> <img src="/resources/google/dns/dns-zone-labels-added/step3.png"/>
4. From the panel at the top of the page, click on "Labels".</br> <img src="/resources/google/dns/dns-zone-labels-added/step4.png"/>
5. A popup will open on the right side of the page, check if there are any labels shown in it. If not, the DNS zone does not have labels added. </br> <img src="/resources/google/dns/dns-zone-labels-added/step5.png"/>
5. Repeat steps number 3-5 to check other zones in the project.</br>
6. Navigate to "Network Services", choose "Cloud DNS". Click on the checkbox next to the name of the "DNS Zone" which needs to have labels added and click on "Labels" at the top of the page.</br> <img src="/resources/google/dns/dns-zone-labels-added/step4.png"/>
7. In the popup on the right side, click on "Add Label" and add key and value for the label. Add as many labels as you want and then click "Save".</br> <img src="/resources/google/dns/dns-zone-labels-added/step7.png"/>
8. Repeat steps number 6-7 to add labels to all other zones in the project.</br>