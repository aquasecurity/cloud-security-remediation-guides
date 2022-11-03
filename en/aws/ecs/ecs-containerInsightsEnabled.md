[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / ECS / ECS Container Insights Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Container Insights Enabled |
| **Cloud** | AWS |
| **Category** | ECS |
| **Description** | Ensure that ECS clusters have CloudWatch Container Insights feature enabled. |
| **More Info** | CloudWatch Container Insights provides monitoring and troubleshooting solution for containerized applications and microservices that collects, aggregates and summarizes resource utilization such as CPU, memory, disk, and network.|
| **AWS Link** | https://docs.aws.amazon.com/AmazonECS/latest/developerguide/cloudwatch-container-insights.html |
| **Recommended Action** | Enable container insights feature for ECS clusters. |

## Detailed Remediation Steps
<b>Setting up Container Insights on new Amazon ECS Cluster</b>
1. Log into the AWS Management Console.
2. Select the "Services" option and search for ECS. </br> <img src="/resources/aws/ecs/ecsContainerInsightsEnabled/step2.png"/>
3. In navigation panel select "Account Settings".</br> <img src="/resources/aws/ecs/ecsContainerInsightsEnabled/step3.png"/>
4. Select the "checkbox" at the bottom of page to enable Container Insights. </br> <img src="/resources/aws/ecs/ecsContainerInsightsEnabled/step4.png"/>

<b>Setting up Container Insights on existing Amazon ECS Cluster</b>
1. To enable Container Insights on existing Amazon ECS cluster, enter the following command. You must be running version 1.16.200 or later of AWS CLI for following command to work</br> <img src="/resources/aws/ecs/ecsContainerInsightsEnabled/step5.png"/>


