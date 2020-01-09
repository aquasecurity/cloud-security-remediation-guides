[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Load Balancer / LB No Instances

## Quick Info

| | |
|-|-|
| **Plugin Title** | LB No Instances |
| **Cloud** | AZURE |
| **Category** | Load Balancer |
| **Description** | Detects load balancers that have no backend instances attached |
| **More Info** | All load balancers should have backend server resources. Those without any are consuming costs without providing any functionality. Additionally, old load balancers with no instances pose a security concern if new instances are accidentally attached. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/load-balancer/load-balancer-overview |
| **Recommended Action** | Delete old load balancers that no longer have backend resources. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Load balancers. </br> <img src="/resources/azure/loadbalancer/lb-no-instances/step2.png"/>
3. Select the "Load balancer" by clicking on the "Name" as a link which needs to be checked for active Instances.</br> <img src="/resources/azure/loadbalancer/lb-no-instances/step3.png"/>
4. On the "Load balancer" page, scroll down the left navigation panel and choose the "Backend pools" option. </br>  <img src="/resources/azure/loadbalancer/lb-no-instances/step4.png"/>
5. On the "Load balancers- Backend pools" page, check whether it has any active Instances or not. If load balancers have no backend instances attached then we can delete it for security concerns.</br>  <img src="/resources/azure/loadbalancer/lb-no-instances/step5.png"/>
6. Repeat steps number 2 - 5 to verify "Load balancer" with no instances.</br>
7. Navigate to "Load balancers", select the load balancer which needs to be deleted. </br> <img src="/resources/azure/loadbalancer/lb-no-instances/step7.png"/>
8. On the selected "Load balancer" click on the "... (three dots)" at extreme right and select "Delete" option.</br> <img src="/resources/azure/loadbalancer/lb-no-instances/step8.png"/>
9. On the "Delete load balancer" tab, click on the "Yes" button to make the changes.</br> <img src="/resources/azure/loadbalancer/lb-no-instances/step9.png"/>
10. Repeat steps number 7 - 9 to delete old load balancers that no longer have backend resources as they are consuming costs without providing any functionality and old load balancers with no instances pose a security concern if new instances are accidentally attached.

