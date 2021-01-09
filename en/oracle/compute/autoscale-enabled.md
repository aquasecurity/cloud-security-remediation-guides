[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Compute / Autoscale Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Autoscale Enabled |
| **Cloud** | ORACLE |
| **Category** | Compute |
| **Description** | Ensures autoscaling is enabled on instance pools. |
| **More Info** | Enabling autoscaling increases efficiency and improves cost management for resources. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Compute/Tasks/autoscalinginstancepools.htm |
| **Recommended Action** | Enable autoscaling on all instance pools |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Instances" under the "Compute." </br> <img src="/resources/oracle/compute/autoscale-enabled/step2.png"/>
3. On the "Instances" page, scroll down and click on the "Autoscaling configurations" option at the left.</br> <img src="/resources/oracle/compute/autoscale-enabled/step3.png"/>
4. On the "Autoscaling configurations" page, check if there is any configuration already there or not. If not then it's not as best recommended practices by Oracle.</br> <img src="/resources/oracle/compute/autoscale-enabled/step4.png"/>
5. Repeat steps 2 - 4 to check other accounts.</br>
6. Navigate to "Instances" under the "Compute" and select the "Autoscaling configurations" option to enable the "Autoscaling" for better efficiency and cost management.</br> <img src="/resources/oracle/compute/autoscale-enabled/step6.png"/>
7. On the "Autoscaling configurations" page, click on the "Create Autoscaling Configuration" button at the top.</br> <img src="/resources/oracle/compute/autoscale-enabled/step7.png"/>
8. On the "Create Autoscaling Configuration" tab, enter the "AUTOSCALING CONFIGURATION NAME" and enter the cooldown period as per requirement.</br> <img src="/resources/oracle/compute/autoscale-enabled/step8.png"/>
9. Under the "Autoscaling configurations", select the "Autoscaling Policy" and select the "Performance Metric" as per the requirement from the dropdown. Also select the "MINIMUM NUMBER OF INSTANCES", "MAXIMUM NUMBER OF INSTANCES" and "INITIAL NUMBER OF INSTANCES" as per the business need.</br> <img src="/resources/oracle/compute/autoscale-enabled/step9.png"/>
10. On the "Scaling Rule" tab, enter the value for "SCALE-IN OPERATOR" and "SCALE-OUT OPERATOR" as "Threshold Percentage" and click on the "Save" button to make the changes.</br> <img src="/resources/oracle/compute/autoscale-enabled/step10.png"/>
11. Repeat steps number 6 - 10 to ensure Autoscaling is enabled on Instance Pools.</br>
