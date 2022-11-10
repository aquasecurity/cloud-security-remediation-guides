[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Apigateway / Custom Domain TLS Version

## Quick Info

|                        |                                                                                                                                                                                          |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Plugin Title**       | Custom Domain TLS Version                                                                                                                                                                |
| **Cloud**              | AWS                                                                                                                                                                                      |
| **Category**           | Api Gateway                                                                                                                                                                              |
| **Description**        | Ensure API Gateway Custom Domains are using current minimum TLS version.                                                                                                                 |
| **More Info**          | A security policy is a predefined combination of minimum TLS version and cipher suite offered by Amazon API Gateway. Choose either a TLS version 1.2 or TLS version 1.0 security policy. |
| **AWS Link**           | https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-custom-domain-tls-version.html                                                                                   |
| **Recommended Action** | Modify API Gateway Custom Domain security policy and specify new TLS version.                                                                                                            |

## Detailed Remediation Steps

1. Log into the AWS Management Console.
2. Select the "Services" option and search for Api Gateway. </br> <img src="/resources/aws/apigateway/custom-domain-tls-version/step2.jpg"/>
3. In the left navigation panel click on "Custom domain names". </br> <img src="/resources/aws/apigateway/custom-domain-tls-version/step3.jpg"/>
4. On the "Custom domain names" page, click on the domain name. From the "Domain Details" page that opens, check if the TLS version is set to current minimum version. </br> <img src="/resources/aws/apigateway/custom-domain-tls-version/step4.jpg">
5. If not, then click on "Edit". On the "Edit domain details" page, choose the minimum latest version (i.e. TLS_1_2). Click on save button to apply changes </br> <img src = "/resources/aws/apigateway/custom-domain-tls-version/step5.jpg">
6. Repeat steps number 4 and 5 to ensure the minimum TLS version for your custom domains.
