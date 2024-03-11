[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / API Gateway / API Gateway Private Endpoints

## Quick Info

| | |
|-|-|
| **Plugin Title** | API Gateway Private Endpoints |
| **Cloud** | AWS |
| **Category** | API Gateway |
| **Description** | Ensures that Amazon API Gateway APIs are only accessible through private endpoints. |
| **More Info** | API Gateway APIs should be only accessible through private endpoints to ensure API security |
| **AWS Link** | https://aws.amazon.com/blogs/compute/introducing-amazon-api-gateway-private-endpoints |
| **Recommended Action** | Set API Gateway API endpoint configuration to private |

## Detailed Remediation Steps
To convert a public endpoint from regional or edge-optimized to Private: </br>
1. Sign in to the API Gateway console at https://console.aws.amazon.com/apigateway. </br>
2. Choose an existing API. </br>
3. Choose Settings. </br>
4. Change the Endpoint Type option under Endpoint Configuration from Edge Optimized or from Regional to Private. </br>
5. You need to specify one or more VPC endpoints with your API and API Gateway will generate new Route 53 Alias records which you can use to invoke your API. </br>
6. If you don't have a VPC, then create one and then Create the VPC endpoint for API Gateway. See this for more details: https://aws.amazon.com/blogs/compute/introducing-amazon-api-gateway-private-endpoints/ </br>
7. Choose Save Changes to start the update. </br>