[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / SageMaker / Notebook Direct Internet Access

## Quick Info

| | |
|-|-|
| **Plugin Title** | Notebook Direct Internet Access |
| **Cloud** | AWS |
| **Category** | SageMaker |
| **Description** | Ensure Notebook Instance is not publicly available. |
| **More Info** | SageMaker notebooks should not be exposed to the Internet. Public availability can be configured via the DirectInternetAccess attribute. |
| **AWS Link** | https://docs.aws.amazon.com/sagemaker/latest/dg/appendix-additional-considerations.html#appendix-notebook-and-internet-access |
| **Recommended Action** | Disable DirectInternetAccess for each SageMaker notebook. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for Sagemaker. </br> <img src="/resources/aws/sagemaker/notebook-direct-internet-access/step2.png"/>
3. Scroll down the left navigation panel and choose the "Notebook instances" under "Notebook" in Amazon Sagemaker.</br> <img src="/resources/aws/sagemaker/notebook-direct-internet-access/step3.png"/>
4.  Select the "Notebook instance" that needs to be verified and click on the "Name" to access the selected "Notebook instance" configuration.</br> <img src="/resources/aws/sagemaker/notebook-direct-internet-access/step4.png"/>
5. On the selected "Notebook instance" configuration page scroll down and check the "Network" tab. If "Direct internet access" is set to "Enabled" then the selected "Notebook instance" is exposed to the Internet. </br> <img src="/resources/aws/sagemaker/notebook-direct-internet-access/step5.png"/>
6. Repeat step number 2 - 5 to verify other "Notebook instances" in the selected AWS region.</br>

