# AWS / CloudFront / CloudFront Geo Restriction

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudFront Geo Restriction |
| **Cloud** | AWS |
| **Category** | CloudFront |
| **Description** | Ensure that geo-restriction feature is enabled for your CloudFront distribution to allow or block location-based access. |
| **More Info** | AWS CloudFront geo restriction feature can be used to assist in mitigation of Distributed Denial of Service (DDoS) attacks. Also you have the ability to block IP addresses based on Geo IP from reaching your distribution and your web application content delivered by the distribution. |
| **AWS Link** | https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/georestrictions.html |
| **Recommended Action** | Enable CloudFront geo restriction to whitelist or block location-based access. |

## Detailed Remediation Steps
To add geographic restrictions to your CloudFront web distribution (console):
1. Sign in to the AWS Management Console.
2. Select the "Services" option and search for CloudFront.
3. In the navigation pane, choose Distributions, then choose the distribution that you want to update.
4. Choose the Security tab, then choose Geographic restrictions.</br> <img src="/resources/aws/cloudfront/cloudfront-geo-restriction/step4.png"/>
5. Choose Edit.
6. Select Allow list to create a list of allowed countries, or Block list to create a list of blocked countries.
7. Add the desired countries to the list, then choose Save changes.

