[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ELB / ELBv2 Insecure Ciphers

## Quick Info

| | |
|-|-|
| **Plugin Title** | ELBv2 Insecure Ciphers |
| **Cloud** | AWS |
| **Category** | ELBv2 |
| **Description** | Ensure that Elbv2 listeners are configured to use the predefined security policies containing secure ciphers. |
| **More Info** | A security policy is a combination of protocols and ciphers. The protocol establishes a secure connection between a client and a server and ensures that all data passed between the client and your load balancer is private. |
| **AWS Link** | https://docs.aws.amazon.com/elasticloadbalancing/latest/network/create-tls-listener.html |
| **Recommended Action** | Modify ELBv2 listeners with the predefined AWS security policies containing secure ciphers. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/elbv2/elbv2-insecure-ciphers/step2.png"/>
3. In the "EC2 Dashboard" scroll down and look for "Load Balancers" and click on "Load Balancers" to get into "Load Balancers" dashboard.</br> <img src="/resources/aws/elbv2/elbv2-insecure-ciphers/step3.png"/>
4. Select the "Load Balancer" of the type application/network, which needs to be verified. </br> <img src="/resources/aws/elbv2/elbv2-insecure-ciphers/step4.png"/>
5. Select the "Listeners" tab from the bottom panel and click on the listener which needs to be updated. </br> <img src="/resources/aws/elbv2/elbv2-insecure-ciphers/step5.png"/>
6. On the new "Listener Details" page, click on edit to update the "Security Policy". </br> <img src="/resources/aws/elbv2/elbv2-insecure-ciphers/step6.png">
7. On "Edit listeners" page that appears update the security policy to latest SSL policy which contains secure ciphers and click on save. </br><img src="/resources/aws/elbv2/elbv2-insecure-ciphers/step7.png"/>
8. Repeat the step number 5 to 7 for each listener on the elbv2. </br>
9. Repeat the step number 4 to 8 for each elbv2, to ensure that all the listeners are using latest security policies which contains secure ciphers.