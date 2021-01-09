[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Compute / Instance Monitoring Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Instance Monitoring Enabled |
| **Cloud** | ORACLE |
| **Category** | Compute |
| **Description** | Ensures monitoring is enabled for instances. |
| **More Info** | Enabling instance monitoring allows for metrics to be collected on the instance. Following security best practices.  |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/Compute/Tasks/enablingmonitoring.htm |
| **Recommended Action** | When creating a new instance, ensure monitoring is enabled under advanced settings. |

## Detailed Remediation Steps
1. Log in to the Oracle Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Instances" under the "Compute." </br> <img src="/resources/oracle/compute/instance-monitoring-enabled/step2.png"/>
3. On the "Instance" page, select the "Instance" in which monitoring needs to be enabled and click on the "Name" as a link to access the configuration settings.</br> <img src="/resources/oracle/compute/instance-monitoring-enabled/step3.png"/>
4. On the "Instances page", scroll down and click on the "Boot Voulmes" under the "Resources."</br> <img src="/resources/oracle/compute/instance-monitoring-enabled/step4.png"/>
5. On the "Boot Volume Page", click on the "Name" as a link to access the "Boot Volume Details" page.</br> <img src="/resources/oracle/compute/instance-monitoring-enabled/step5.png"/>
6. On the "Boot Volume Details" page, scroll down and click on the "Boot Volume Clones" under the "Resources."</br> <img src="/resources/oracle/compute/instance-monitoring-enabled/step6.png"/>
7. On the "Boot Volume Clones" tab, click on the 3dots at the extreme right and click on the "Create Instance" option.</br> <img src="/resources/oracle/compute/instance-monitoring-enabled/step7.png"/>
8. On the "Create Compute Instance" page, scroll down and click on the "Show Advanced Options."</br> <img src="/resources/oracle/compute/instance-monitoring-enabled/step8.png"/>
9. On the "Advanced Options" tab, and in the "Management" section, click on the checkbox next to "ENABLE MONITORING" under the "Oracle Cloud Agent" and click on the "Create" button to finish the process.</br>  <img src="/resources/oracle/compute/instance-monitoring-enabled/step9.png"/>
10. Repeat steps number 2 - 10 to enable instance monitoring.</br>
