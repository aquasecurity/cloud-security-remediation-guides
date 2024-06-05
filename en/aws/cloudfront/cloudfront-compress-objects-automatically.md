# AWS / CloudFront / CloudFront Compress Objects Automatically

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudFront Compress Objects Automatically |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Ensure that your Amazon CloudFront distributions are configured to automatically compress files (object). |
| **More Info** | CloudFront data transfer is based on the total amount of data served, sending compressed files to the viewers is much less expensive than sending uncompressed files. To optimize your AWS cloud costs and speed up your web applications, configure your CloudFront distributions to compress the web content served with compression enabled. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/ServingCompressedFiles.html |
| **Recommended Action** | Ensures that CloudFront is configured to automatically compress files. |

## Detailed Remediation Steps
To configure CloudFront to compress objects, update the cache behavior that you want to serve the compressed objects by doing all of the following:

1. Sign in to the AWS Management Console.
2. Select the "Services" option and search for CloudFront.
3. In the left navigation panel, under CloudFront, choose Distributions.
4. Click on the name of the Amazon CloudFront distribution that you want to edit.
5. Select the Behaviors tab to access the cache behavior(s) configured for the selected distribution.</br> <img src="/resources/aws/cloudfront/cloudfront-compress-objects-automatically/step5.png"/>
6. Select the cache behavior that you want to examine and choose Edit.
7. On the Edit behavior configuration page, check the Compress objects automatically configuration setting. </br> <img src="/resources/aws/cloudfront/cloudfront-compress-objects-automatically/step7.png"/>

**Note**: In AWS CloudFormation or the CloudFront API, set Compress to true.


