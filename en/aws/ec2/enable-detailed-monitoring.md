[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Enable Detailed Monitoring

# Quick Info

|                        |                                                                                                                                                                                                                                            |
| - | - |
| **Plugin Title**       | Instance Detailed Monitoring                                                                                                                                                                                                               |
| **Cloud**              | AWS                                                                                                                                                                                                                                        |
| **Category**           | EC2                                                                                                                                                                                                                                        |
| **Description**        | Ensure that EC2 instances have detailed monitoring feature enabled.                                                                                                                                                                        |
| **More Info**          | By default, your instance is enabled for basic monitoring. You can optionally enable detailed monitoring. After you enable detailed monitoring, the Amazon EC2 console displays monitoring graphs with a 1-minute period for the instance. |
| **AWS Link**           | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-cloudwatch-new.html                                                                                                                                                              |
| **Recommended Action** | Modify EC2 instance to enable detailed monitoring.                                                                                                                                                                                         |

## Detailed Remediation Steps

1. Log into the AWS Management Console.
2. Select the "Services" option and search for EC2. </br> <img src="/resources/aws/ec2/enable-detailed-monitoring/step2.png"/>
3. Scroll down the left navigation panel and choose "Instances" under the "Instances"
   <img src="/resources/aws/ec2/enable-detailed-monitoring/step3.png"/>
4. Select the "EC2 Instance" that needs to have detailed monitoring enable. <img src="/resources/aws/ec2/enable-detailed-monitoring/step4.png"/>
5. In the tab down below switch to "Monitoring" Tab, and click on "Manage Detailed Monitoring" on the top right corner. <img src="/resources/aws/ec2/enable-detailed-monitoring/step5.png"/>
6. Enable the detailed monitoring on the pop-up and hit confirm <img src="/resources/aws/ec2/enable-detailed-monitoring/step6.png"/>
7. Repeat the steps 4,5,6 for each instance.
