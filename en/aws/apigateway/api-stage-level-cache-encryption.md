[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / API Gateway / API Stage-Level Cache Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | API Stage-Level Cache Encryption |
| **Cloud** | AWS |
| **Category** | API Gateway |
| **Description** | Ensure that your Amazon API Gateway REST APIs are configured to encrypt API cached responses. |
| **More Info** | It is strongly recommended to enforce encryption for API cached responses in order to protect your data from unauthorized access. |
| **AWS Link** | https://docs.aws.amazon.com/apigateway/latest/developerguide/data-protection-encryption.html |
| **Recommended Action** | Modify API Gateway API stages to enable encryption on cache data |

## Detailed Remediation Steps
To configure API caching for individual methods using the console: </br>
1. Sign in to the API Gateway console at https://console.aws.amazon.com/apigateway. </br>
2. Go to the API Gateway console. </br>
3. Choose the API. </br>
4. Choose Stages. </br>
5. In the Stages list for the API, expand the stage and choose a method in the API. </br>
6. Choose Override for this method in Settings. </br>
7. In Cache Settings, choose Encrypt cache data. (This section is shown only if stage-level caching is enabled.) </br>