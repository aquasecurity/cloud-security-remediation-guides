[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Cloud Functions / HTTP Trigger require HTTPS

## Quick Info

| | |
|-|-|
| **Plugin Title** | HTTP Trigger require HTTPS |
| **Cloud** | GOOGLE |
| **Category** | Cloud Functions |
| **Description** | Ensure that Cloud Functions are configured to require HTTPS for HTTP invocations. |
| **More Info** | You can make your google cloud functions call secure by making sure that they require HTTPS. |
| **GOOGLE Link** | https://cloud.google.com/functions/docs/writing/http |
| **Recommended Action** | Ensure that your Google Cloud functions always require HTTPS. |

## Detailed Remediation Steps
In Cloud Functions (2nd gen), requests to a function URL always require HTTPS. In Cloud Functions (1st gen), you can choose whether HTTPS is required during deployment.
Steps to configure Cloud Functions to require HTTPS:
a. Using gcloud:
   1. (1st gen) Set `--security-level` flag value to `secure-always` which means HTTPS is required and non-SSL HTTP requests are not supported. 
   Example: 
   ```
   gcloud functions deploy YOUR_FUNCTION_NAME \
--trigger-http \
[--allow-unauthenticated] \
[--security-level=secure-always] \
...
   ```
b. Using Console
For Cloud Functions (1st gen):
    1. Log into the Google Cloud Platform Console.
    2. Scroll down the left navigation panel and click on "Cloud Functions". </br> <img src="/resources/google/cloudfunctions/http-trigger-require-https/step2.png"></br>
    3. On the "Cloud Functions" page, select the cloud function which needs to change to require https by clicking on the checkbox next to its name.</br> <img src="/resources/google/cloudfunctions/http-trigger-require-https/step4.png"/></br>
    4. In the Trigger type field, select HTTP. </br><img src="/resources/google/cloudfunctions/http-trigger-require-https/step5.png"/></br>
    5. Select the Require HTTPS checkbox to make the function endpoint requires HTTPS.</br><img src="/resources/google/cloudfunctions/http-trigger-require-https/step6.png"/></br>
    For more info: https://cloud.google.com/functions/docs/calling/http#gcloud