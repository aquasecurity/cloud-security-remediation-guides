# AWS / CloudFront / CloudFront Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudFront Enabled |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Ensure that AWS CloudFront service is used within your AWS account. |
| **More Info** | Amazon CloudFront is a web service that speeds up distribution of your static and dynamic web content, such as .html, .css, .js, and image files, to your users. CloudFront delivers your content through a worldwide network of data centers called edge locations.  |
| **AWS Link** | https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html |
| **Recommended Action** | Create CloudFront distributions as per requirements. |

## Detailed Remediation Steps
How to create and configure CloudFront to deliver your content
1. Sign in to the AWS Management Console.
2. Select the "Services" option and search for CloudFront. </br> <img src="/resources/aws/cloudfront/cloudfront-enabled/step2.png"/>
3. In the left navigation panel, under CloudFront, choose Distributions.</br> <img src="/resources/aws/cloudfront/cloudfront-enabled/step3.png"/>
4. Choose Create distribution.</br> <img src="/resources/aws/cloudfront/cloudfront-enabled/step4.png"/>
5. On the Create distribution page specify origin servers, like an Amazon S3 bucket or your own HTTP server, from which CloudFront gets your files which will then be distributed from CloudFront edge locations all over the world. Your HTTP server can run on an Amazon Elastic Compute Cloud (Amazon EC2) instance or on a server that you manage; these servers are also known as custom origins. 
The CloudFront distribution tells CloudFront which origin servers to get your files from when users request the files through your web site or application. At the same time, you specify details such as whether you want CloudFront to log all requests and whether you want the distribution to be enabled as soon as it's created.</br> <img src="/resources/aws/cloudfront/cloudfront-enabled/step4.png"/>.
6. Under Default cache behavior Sectoin:
    a. Choose Yes under Compress objects automatically to enable Amazon CloudFront to automatically compress certain files that it receives from the origin before delivering them to the viewer.


