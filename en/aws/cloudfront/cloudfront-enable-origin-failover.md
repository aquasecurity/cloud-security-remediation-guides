# AWS / CloudFront / CloudFront Enable Origin Failover

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudFront Enable Origin Failover |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Ensure that Origin Failover feature is enabled for your CloudFront distributions in order to improve the availability of the content delivered to your end users. |
| **More Info** | With Origin Failover capability, you can setup two origins for your CloudFront web distributions primary and secondary. In the event of primary origin failure, your content is automatically served from the secondary origin, maintaining the distribution high reliability.  |
| **AWS Link** | https://docs.aws.amazon.com/cloudfront/latest/APIReference/API_OriginGroupFailoverCriteria.html |
| **Recommended Action** | Modify CloudFront distributions and configure origin group instead of a single origin. |

## Detailed Remediation Steps
You can set up CloudFront with origin failover for scenarios that require high availability. To get started, you create an origin group with two origins: a primary and a secondary. If the primary origin is unavailable, or returns specific HTTP response status codes that indicate a failure, CloudFront automatically switches to the secondary origin.

To set up origin failover, you must have a distribution with at least two origins. Next, you create an origin group for your distribution that includes two origins, setting one as the primary. Finally, you create or update a cache behavior to use the origin group.

Steps for setting up origin groups and configuring specific origin failover options:

1. Sign in to the AWS Management Console.
2. Select the "Services" option and search for CloudFront.
3. Choose the distribution that you want to create the origin group for.
4. Choose the Origins tab.
5. Make sure the distribution has more than one origin. If it doesn’t, add a second origin.
6. On the Origins tab, in the Origin groups pane, choose Create origin group.</br> <img src="/resources/aws/cloudfront/cloudfront-enable-origin-failover/step6.png"/>
7. Choose the origins for the origin group. After you add origins, use the arrows to set the priority—that is, which origin is primary and which is secondary.
8. Enter a name for the origin group.
9. Choose the HTTP status codes to use as failover criteria. You can choose any combination of the following status codes: 400, 403, 404, 416, 500, 502, 503, or 504. When CloudFront receives a response with one of the status codes that you specify, it fails over to the secondary origin.
10. Choose Create origin group.</br> <img src="/resources/aws/cloudfront/cloudfront-enable-origin-failover/step10.png"/>
**Note**
 If you created cache behaviors in addition to the default cache behavior, make sure to assign your origin group as the origin for your distribution's cache behavior. For more information, see [Name](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/distribution-web-values-specify.html#DownloadDistValuesId).

