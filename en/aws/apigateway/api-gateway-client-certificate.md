[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / API Gateway / API Gateway Client Certificate

## Quick Info

| | |
|-|-|
| **Plugin Title** | API Gateway Client Certificate |
| **Cloud** | AWS |
| **Category** | API Gateway |
| **Description** | Ensures that Amazon API Gateway API stages use client certificates |
| **More Info** | API Gateway API stages should use client certificates to ensure API security authorization. |
| **AWS Link** | https://docs.aws.amazon.com/apigateway/latest/developerguide/getting-started-client-side-ssl-authentication.html |
| **Recommended Action** | Attach client certificate to API Gateway API stages |

## Detailed Remediation Steps
Generate a client certificate using the API Gateway console: </br>
1. Open the API Gateway console at https://console.aws.amazon.com/apigateway/. </br>
2. Choose a REST API.
3. In the main navigation pane, choose Client Certificates. </br>
4. From the Client Certificates pane, choose Generate Client Certificate. </br>
5. Optionally, for Edit, choose to add a descriptive title for the generated certificate and choose Save to save the description. API Gateway generates a new certificate and returns the new certificate GUID. </br>

Now you need to configure an API to use SSL certificate:
1. In the API Gateway console, create or open an API for which you want to use the client certificate. Make sure that the API has been deployed to a stage. For more information on how to deploy see https://docs.aws.amazon.com/apigateway/latest/developerguide/how-to-deploy-api-with-console.html#how-to-deploy-api-console </br>
2. Choose Stages under the selected API and then choose a stage. </br>
3. In the Stage Editor panel, select a certificate under the Client Certificate section. </br>
4. To save the settings, choose Save Changes. </br>
5. If the API has been deployed previously in the API Gateway console, you'll need to redeploy it for the changes to take effect. For more information, see https://docs.aws.amazon.com/apigateway/latest/developerguide/how-to-deploy-api-with-console.html#apigateway-how-to-redeploy-api-console </br>