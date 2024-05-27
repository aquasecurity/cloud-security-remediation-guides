[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Load Balancer / Public Load Balancer

## Quick Info

| | |
|-|-|
| **Plugin Title** | Public Load Balancer |
| **Cloud** | AZURE |
| **Category** | Load Balancer |
| **Description** | Ensures that Azure Load Balancers are configured as public. |
| **More Info** | To meet your organization\'s security compliance, ensure that load balancers are public to facilitate efficient egress to the Internet for backend pool members through the assigned frontend IP, ensuring streamlined connectivity and reliable resource availability. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/load-balancer/load-balancer-overview |
| **Recommended Action** | Create the Load Balancer with Ip associations as per your organization\'s requirements. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. In search bar at the top search for Load balancers and select "Load Balancers". </br> <img src="/resources/azure/loadbalancer/lb-public-ip/step2.png"/>
3. Click on the  Create Load balancer option at the top.</br> <img src="/resources/azure/loadbalancer/lb-public-ip/step3.png"/>
4. On the Create load balancer creation page, you will see two type public or internal , choose the type according to your organization's requirements. </br> <img src="/resources/azure/loadbalancer/lb-public-ip/step4.png"/>
5. check on 'Next: Frontend IP Configuration' at the bottom , to add the IP association to your Load balancer. </br> <img src="/resources/azure/loadbalancer/lb-public-ip/step5.png"/>
6. Click on 'Add a frontend IP configuration' at the top to add the IP configuration. </br> <img src="/resources/azure/loadbalancer/lb-public-ip/step6.png"/>
7. In case of Public Load balancer, add the name, IP version, IP type , public IP address as per your choice and click the save button to save the IP configuration. </br> <img src="/resources/azure/loadbalancer/lb-public-ip/step7.png"/>
8. In case of Internal Load balancer, add the name, IP version and select the virtual network as per your choice and save the IP configuration .</br> <img src="/resources/azure/loadbalancer/lb-public-ip/step8.png"/>
9. Add the IP configuration and then click on the 'Next: Backend Pools' and fill the options as per requirement to create the Load balancer. <img src="/resources/azure/loadbalancer/lb-public-ip/step9.png"/>
10. Click on 'Create' button to create the Load balancer with IP configuration as per your organization requiremnets. <img src="/resources/azure/loadbalancer/lb-public-ip/step10.png"/>