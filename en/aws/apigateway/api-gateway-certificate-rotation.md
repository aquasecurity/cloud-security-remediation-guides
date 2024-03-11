[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / API Gateway / API Gateway Certificate Rotation

## Quick Info

| | |
|-|-|
| **Plugin Title** | API Gateway Certificate Rotation |
| **Cloud** | AWS |
| **Category** | API Gateway |
| **Description** | Ensures that Amazon API Gateway APIs have certificates with expiration date more than the rotation limit. |
| **More Info** | API Gateway APIs should have certificates with long term expiry date to avoid API insecurity after certificate expiration. |
| **AWS Link** | https://docs.aws.amazon.com/apigateway/latest/developerguide/data-protection-encryption.html |
| **Recommended Action** | Rotate the certificate attached to API Gateway API |

## Detailed Remediation Steps
You must rotate the certificate before a client certificate on an API stage expires to avoid any downtime for the API. </br>
To rotate a client certificate in the console for a previously deployed API, do the following: </br>
1. Open the API Gateway console at https://console.aws.amazon.com/apigateway/. </br>
2.  In the main navigation pane, choose Client Certificates. </br>
3. From the Client Certificates pane, choose Generate Client Certificate. </br>
4. From navigation pane again click on APIs. </br>
5. Open the API for which you want to use the client certificate. </br>
6. Choose Stages under the selected API and then choose a stage. </br>
7. In the Stage Editor panel, select the new certificate under the Client Certificate section. </br>
8. To save the settings, choose Save Changes. </br>