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
2. In search bar at the top search for Load balancers and select "Load Balancers". </br> <img src="/resources/azure/loadbalancer/lb-no-instances/step2.png"/>
3. Select the "Load balancer" by clicking on the "Name" as a link which needs to be checked for active Instances.</br> <img src="/resources/azure/loadbalancer/lb-no-instances/step3.png"/>
4. On the "Load balancer" page, scroll down the left navigation panel and choose the "Backend pools" option. </br>  <img src="/resources/azure/loadbalancer/lb-no-instances/step4.png"/>
5. On the "Backend pools" pane that opens, if there are no backend instances then we should delete it as a security best practice.</br>  <img src="/resources/azure/loadbalancer/lb-no-instances/step5.png"/>
6. In the left navigation panel click on "Overview" and click on "Delete" button at the top to delete the load balancer.</br>  <img src="/resources/azure/loadbalancer/lb-no-instances/step6.png"/>
7. In the confimation box that opens, click "Yes" to confirm deletion of this load balancer.</br>  <img src="/resources/azure/loadbalancer/lb-no-instances/step7.png"/>
10. Repeat step number 3 - 7 to check and delete old load balancers that no longer have backend resources.
