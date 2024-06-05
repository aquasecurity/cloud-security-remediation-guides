# AWS / CloudFront / CloudFront Custom Origin HTTPS Only

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudFront Custom Origin HTTPS Only |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Ensures CloudFront Distribution Custom Origin is HTTPS Only. |
| **More Info** | When you create a distribution, you specify the origin where CloudFront sends requests for the files. You can use several different kinds of origins with CloudFront. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/using-https-cloudfront-to-custom-origin.html |
| **Recommended Action** | Modify CloudFront distribution and update the Origin Protocol Policy setting to HTTPS Only. |

## Detailed Remediation Steps
To configure CloudFront to require HTTPS between CloudFront and your custom origin:
1. Sign in to the AWS Management Console.
2. Select the "Services" option and search for CloudFront.
3. In the left navigation panel, under CloudFront, choose Distributions.
4. Click on the name of the Amazon CloudFront distribution that you want to update.
5. On the Behaviors tab, select the origin that you want to update, and then choose Edit
6. Update the viewer protocol policy to use HTTPS only.</br> <img src="/resources/aws/cloudfront/cloudfront-custom-origin-https-only/step6.png"/>
7. Choose Save changes.
8. Repeat steps 5 through 7 for each additional origin that you want to require HTTPS for between CloudFront and your custom origin.


