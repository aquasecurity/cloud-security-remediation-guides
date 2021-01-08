[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Autoscale Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Autoscale Enabled |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensures instance groups have autoscale enabled for high availability |
| **More Info** | Enabling autoscale increases efficiency and improves cost management for resources. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/autoscaler/ |
| **Recommended Action** | Ensure autoscaling is enabled for all instance groups. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Compute Engine" to select the "Instance groups" option. </br> <img src="/resources/google/compute/autoscale-enabled/step2.png"/>
3. On the "Instance groups" page, select the instance group which needs to be verified whether autoscale is enabled or not by clicking on the "Name" as a link.</br> <img src="/resources/google/compute/autoscale-enabled/step3.png"/>
4. On the "Instance groups" page, if a popup stated autoscale is turned off then the selected instance group don't have autoscale enabled for high availability.</br> <img src="/resources/google/compute/autoscale-enabled/step4.png"/>
5. Repeat steps number 2 - 4 to check other "Instance group" in the account.</br>
6. Navigate to "Compute Engine", choose the "Instance groups" and select the "Instance group" which needs to enabled "Autoscale" for high availability.</br> <img src="/resources/google/compute/autoscale-enabled/step6.png"/>
7. On the "Instance group" page, select the group by clicking on the "Name" as a link.</br> <img src="/resources/google/compute/autoscale-enabled/step7.png"/>
8. On the selected "Instance group" page, click on the "Configure auto-scaling" option.</br> <img src="/resources/google/compute/autoscale-enabled/step8.png"/>
9. On the "Configure auto-scaling" page, scroll down the page and on the "Auto-scaling mode" option , choose the "Auto scale" from the drop down menu.</br> <img src="/resources/google/compute/autoscale-enabled/step9.png"/>
10. Click on the "Save" button to make the changes.</br> <img src="/resources/google/compute/autoscale-enabled/step10.png"/>
11. Repeat steps number 6 - 10 to ensure autoscaling is enabled for all the instances groups.</br>
