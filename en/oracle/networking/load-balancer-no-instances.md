[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# ORACLE / Networking / Load Balancer No Instances

## Quick Info

| | |
|-|-|
| **Plugin Title** | Load Balancer No Instances |
| **Cloud** | ORACLE |
| **Category** | Networking |
| **Description** | Detects LBs that have no backend instances attached |
| **More Info** | All LBs should have backend server resources. Those without any are consuming costs without providing any functionality. Additionally, old LBs with no instances present a security concern if new instances are accidentally attached. |
| **ORACLE Link** | https://docs.cloud.oracle.com/iaas/Content/GSG/Tasks/loadbalancing.htm |
| **Recommended Action** | Delete old LBs that no longer have backend resources. |

## Detailed Remediation Steps
1. Log in to the Google Oracle Platform Console.
2. Scroll down the left navigation panel and choose the "Load Balancers" under the "Networking." </br> <img src="/resources/oracle/networking/load-balancer-no-instances/step2.png"/>
3. On the "Load Balancers" page, select the "Load Balancer" by clicking on the "Name" as a link to access the "Load Balancer."</br>  <img src="/resources/oracle/networking/load-balancer-no-instances/step3.png"/>
4. On the "Load Balancer Details" page, scroll down and click on the "Backend sets" under the "Resources".</br>  <img src="/resources/oracle/networking/load-balancer-no-instances/step4.png"/>
5. On the "Backend sets detail" page scroll down and select the "Backends" option from the left menu and check if there is any active "Instance" is attached or not.</br> <img src="/resources/oracle/networking/load-balancer-no-instances/step5.png"/>
6. Repeat steps number 2 - 5 to detects LBs that have no backend instances attached.</br>
7. Navigate to "Load balancers" under the "Networking", select the load balancer with "No Instances."</br> <img src="/resources/oracle/networking/load-balancer-no-instances/step7.png"/>
8. Click on the 3dots at the extreme right to open the "Options" menu. Click on the "Terminate" to remove the "load balancer" without any active Instance.</br> <img src="/resources/oracle/networking/load-balancer-no-instances/step8.png"/>
9. On the "Terminate Load Balancer" tab, click on the "Terminate" button to delete the selected "Load balancer."</br> <img src="/resources/oracle/networking/load-balancer-no-instances/step9.png"/>
10. Repeat steps number 7 - 9 to delete old LBs that no longer have backend resources.</br>
