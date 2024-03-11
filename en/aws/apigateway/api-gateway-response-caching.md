[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / API Gateway / API Gateway Response Caching

## Quick Info

| | |
|-|-|
| **Plugin Title** | API Gateway Response Caching |
| **Cloud** | AWS |
| **Category** | API Gateway |
| **Description** | Ensure that response caching is enabled for your Amazon API Gateway REST APIs. |
| **More Info** | A REST API in API Gateway is a collection of resources and methods that are integrated with backend HTTP endpoints, Lambda functions, or other AWS services.You can enable API caching in Amazon API Gateway to cache your endpoint responses. With caching, you can reduce the number of calls made to your endpoint and also improve the latency of requests to your API. |
| **AWS Link** | https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-caching.html |
| **Recommended Action** | Modify API Gateway API stages to enable API cache |

## Detailed Remediation Steps
To configure API caching for a given stage:
1. Sign in to the API Gateway console at https://console.aws.amazon.com/apigateway. </br>
2. Choose an existing API. </br>
3. Choose Stages. </br>
4. In the Stages list for the API, choose the stage. </br>
5. Choose the Settings tab. </br>
6. Choose Enable API cache. </br>
7. Wait for the cache creation to complete. </br>