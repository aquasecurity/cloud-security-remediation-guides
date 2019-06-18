[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / SageMaker / Notebook Data Encrypted

## Quick Info

| | |
|-|-|
| **Plugin Title** | Notebook Data Encrypted |
| **Cloud** | AWS |
| **Category** | SageMaker |
| **Description** | Ensure Notebook data is encrypted |
| **More Info** | An optional encryption key can be supplied during Notebook Instance creation. |
| **AWS Link** | https://docs.aws.amazon.com/sagemaker/latest/dg/API_CreateNotebookInstance.html#API_CreateNotebookInstance_RequestSyntax |
| **Recommended Action** | An existing KMS key should be supplied during Notebook Instance creation. |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for Sagemaker. </br> <img src="/resources/aws/sagemaker/notebook-data-encrypted/step2.png"/>
3. Scroll down the left navigation panel and choose the "Notebook instances" under "Notebook" in Amazon Sagemaker.</br> <img src="/resources/aws/sagemaker/notebook-data-encrypted/step3.png"/>
4.  Select the "Notebook instance" that needs to be verified and click on the "Name" to access the selected "Notebook instance" configuration.</br> <img src="/resources/aws/sagemaker/notebook-data-encrypted/step4.png"/>
5. On the selected "Notebook instance" configuration page scroll down and check the "Permissions and encryption" tab. If "Encryption key" is not showing any value than the selected "Notebook instance" data is not encrypted.</br> <img src="/resources/aws/sagemaker/notebook-data-encrypted/step5.png"/>
6. Repeat step number 2 - 5 to verify other "Notebook instances" in the selected AWS region.</br>
7. Navigate to "Sagemaker" and select the "Notebook instance" under "Notebook" and click on the "Create notebook instance" to create a new "Notebook instance" with data encrypted.</br> <img src="/resources/aws/sagemaker/notebook-data-encrypted/step7.png"/>
8. On the "Create notebook instance" page provide a unique name under the "Notebook instance name" and select the "Notebook instance type" as per the requirements.</br> <img src="/resources/aws/sagemaker/notebook-data-encrypted/step8.png"/>
9. Scroll down the "Create notebook instance" page and on the "Permissions and encryption" tab select the "IAM role" by either creating a new "IAM role" or entering the "Custom IAM role ARN". Select the "Encryption key" from the dropdown menu.</br> <img src="/resources/aws/sagemaker/notebook-data-encrypted/step9.png"/>
10. Click on the "Create notebook instance" button at the bottom to create a new "Notebook instance".</br> <img src="/resources/aws/sagemaker/notebook-data-encrypted/step10.png"/>
11. Once the new "Notebook instance" status is "InService" copy all the data from old "Notebook instance" to the new instance.</br> <img src="/resources/aws/sagemaker/notebook-data-encrypted/step11.png"/>
12. Repeat steps number 7 - 11 to create the "Notebook instances" with an exisiting "KMS key".</br>

