[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Elastic IP Limit

## Quick Info

| | |
|-|-|
| **Plugin Title** | Elastic IP Limit |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Determine if the number of allocated EIPs is close to the AWS per-account limit |
| **More Info** | AWS limits accounts to certain numbers of resources. Exceeding those limits could prevent resources from launching. |
| **AWS Link** | http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/elastic-ip-addresses-eip.html#using-instance-addressing-limit |
| **Recommended Action** | Contact AWS support to increase the number of EIPs available |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/elastic-ip-limit/step2.png"/>
3. Scroll down the left navigation panel and choose "Elastic IPs" under "Network & Security". </br> <img src="/resources/aws/ec2/elastic-ip-limit/step3.png"/>
4. Check the number of "Elastic IPs" associated within the region.If the selected region has already reached the default limit of 5 Elastic IPs then raise an AWS support ticket to increase the number of "Elastic IPs" in the desired region.</br> <img src="/resources/aws/ec2/elastic-ip-limit/step4.png"/>
5. Repeat steps number 2 - 4 to verify number of "Elastic IPs" associated with other AWS regions.</br>
6. Click on the "Support" option at the top right corner and select the "Support Center".</br> <img src="/resources/aws/ec2/elastic-ip-limit/step6.png"/>
7. In the "Support Center" page click on the "Create Case" button.</br> <img src="/resources/aws/ec2/elastic-ip-limit/step7.png"/>
8. Select the "Service limit increase" tab and choose the "Elastic IPs" from the dropdown in "Limit Type".</br> <img src="/resources/aws/ec2/elastic-ip-limit/step8.png"/>
9. Scroll down the page and select the "Region" and "Limit" as either "EC2-Classic IP Address Limit" or "New VPC IP Address Limit". Provide the "New limit value" as per the requirements. </br> <img src="/resources/aws/ec2/elastic-ip-limit/step9.png"/>
10. Provide a small description to your request in "Case description". </br> <img src="/resources/aws/ec2/elastic-ip-limit/step10.png"/>
11. Select  preferred contact option to the AWS Support team and click on the "Submit" button to increase the "Elastic IPs" request to AWS.</br> <img src="/resources/aws/ec2/elastic-ip-limit/step11.png"/>
 
