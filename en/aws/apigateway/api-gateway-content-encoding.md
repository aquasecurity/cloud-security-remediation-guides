[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / API Gateway / API Gateway Content Encoding

## Quick Info

| | |
|-|-|
| **Plugin Title** | API Gateway Content Encoding |
| **Cloud** | AWS |
| **Category** | API Gateway |
| **Description** | Ensures that Amazon API Gateway APIs have content encoding enabled. |
| **More Info** | API Gateway API should have content encoding enabled to enable compression of response payload. |
| **AWS Link** | https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-gzip-compression-decompression.html |
| **Recommended Action** | Enable content encoding and set minimum compression size of API Gateway API response |

## Detailed Remediation Steps
1. Sign in to the API Gateway console at https://console.aws.amazon.com/apigateway. </br>
2. Choose an existing API. </br>
3. In the primary navigation pane, choose Settings under the API you chose. </br>
4. Under the Content Encoding section in the Settings pane, select the Content Encoding enabled option to enable payload compression. Enter a number for the minimum compression size (in bytes) next to Minimum body size required for compression. </br>
5. Choose Save Changes.</br>