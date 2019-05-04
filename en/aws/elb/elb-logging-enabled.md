[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ELB / ELB Logging Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | ELB Logging Enabled |
| **Cloud** | AWS |
| **Category** | ELB |
| **Description** | Ensures load balancers have request logging enabled. |
| **More Info** | Logging requests to ELB endpoints is a helpful way of detecting and investigating potential attacks, malicious activity, or misuse of backend resources.Logs can be sent to S3 and processed for further analysis. |
| **AWS Link** | http://docs.aws.amazon.com/elasticloadbalancing/latest/application/load-balancer-access-logs.html |
| **Recommended Action** | Enable ELB request logging |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/elb/elb-logging-enabled/step2.png"/>
3. In the "EC2 Dashboard" scroll down and look for "Load Balancers" and click on "Load Balancers" to get into "Load Balancers" dashboard.</br> <img src="/resources/aws/elb/elb-logging-enabled/step3.png"/>
4. Select the "Load Balancer" which needs to be verified. </br> <img src="/resources/aws/elb/elb-logging-enabled/step4.png"/>
5. Select the "Description" tab from the bottom panel and scroll down to "Attributes" option.</br> <img src="/resources/aws/elb/elb-logging-enabled/step5.png"/>
6. Check the "Access logs" and if it's "Disabled" than the "Access logs" feature is not enabled on the selected "Load Balancer". Access Logs delivers detailed logs of all requests made to "Elastic Load Balancing".</br><img src="/resources/aws/elb/elb-logging-enabled/step6.png"/>
7. Click on "Edit attributes" button and click on "Enable" checkbox next to "Access Logs". Specify the S3 location and prefix for the S3 bucket to store the log files and click on "Create this location for me" checkbox so AWS can create a new bucket. If you don't click on "Create this location for me" checkbox provide name of the existing bucket.</br>he selected "Load Balancer". Access Logs delivers detailed logs of all requests made to "Elastic Load Balancing".</br><img src="/resources/aws/elb/elb-logging-enabled/step7.png"/>
8. Click on the "Save" button to make the necessary changes.</br><img src="/resources/aws/elb/elb-logging-enabled/step8.png"/>
9. S3 bucket and Load Balancer needs to exist in the same zone.</br>
10. Selected "Load Balancer" have request logging enabled now. </br> 
