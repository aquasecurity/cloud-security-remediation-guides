[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ELB / ELB HTTPS Only

## Quick Info

| | |
|-|-|
| **Plugin Title** | ELB HTTPS Only |
| **Cloud** | AWS |
| **Category** | ELB |
| **Description** | Ensures ELBs are configured to only accept connections on HTTPS ports. |
| **More Info** | For maximum security, ELBs can be configured to only accept HTTPS connections. Standard HTTP connections  will be blocked. This should only be done if the  client application is configured to query HTTPS  directly and not rely on a redirect from HTTP. |
| **AWS Link** | http://docs.aws.amazon.com/ElasticLoadBalancing/latest/DeveloperGuide/elb-security-policy-options.html |
| **Recommended Action** | Remove non-HTTPS listeners from load balancer. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/elb/elb-https-only/step2.png"/>
3. In the "EC2 Dashboard" scroll down and look for "Load Balancers" and click on "Load Balancers" to get into "Load Balancers" dashboard.</br> <img src="/resources/aws/elb/elb-https-only/step3.png"/>
4. Select the "Load Balancer" which needs to be verified. </br> <img src="/resources/aws/elb/elb-https-only/step4.png"/>
5. Select the "Listeners" tab from the bottom panel and scroll down to the "Load Balancer Protocol" column. Check for "HTTP" under "Instance Protocol". </br> <img src="/resources/aws/elb/elb-https-only/step5.png"/>
6. On the "Listeners" tab scroll down and click on the "Edit" button to remove non-HTTPS listeners.</br><img src="/resources/aws/elb/elb-https-only/step6.png"/>
7. On "Edit listers" tab remove non-HTTPS listeners by clicking on cross icon at the extreme right and click on the "Save" button to make the necessary changes. </br><img src="/resources/aws/elb/elb-https-only/step7.png"/>
8. ELBs are now configured to only accept the connection on HTTPS ports.</br>
