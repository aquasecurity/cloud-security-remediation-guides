[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudTrail / CloudTrail Global Services Logging Duplicated

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudTrail Global Services Logging Duplicated |
| **Cloud** | AWS |
| **Category** | CloudTrail |
| **Description** | Ensures that AWS CloudTrail trails are not duplicating global services events in log files. |
| **More Info** | Only one trail should have Include Global Services feature enabled to avoid duplication of global services events in log files. |
| **AWS Link** | https://docs.aws.amazon.com/IAM/latest/UserGuide/cloudtrail-integration.html |
| **Recommended Action** | Update CloudTrail trails to log global services events enabled for only one trail. |

## Detailed Remediation Steps
For global services such as AWS Identity and Access Management (IAM), AWS STS, and Amazon CloudFront, events are delivered to any trail that includes global services.

To avoid receiving duplicate global service events, remember the following:

1. Global service events are delivered by default to trails that are created using the CloudTrail console. Events are delivered to the bucket for the trail.

2. If you have multiple single Region trails, consider configuring your trails so that global service events are delivered in only one of the trails. 

3. If you change the configuration of a trail from logging all Regions to logging a single Region, global service event logging is turned off automatically for that trail. Similarly, if you change the configuration of a trail from logging a single Region to logging all Regions, global service event logging is turned on automatically for that trail.

**To change global service event logging for a trail:**
To change a trail so that it does not log global service events, use the `--no-include-global-service-events` option.


```
aws cloudtrail update-trail --name my-trail --no-include-global-service-events
```
To confirm that the trail no longer logs global service events, the `IncludeGlobalServiceEvents` element in the output shows `false`.


```
{
    "IncludeGlobalServiceEvents": false, 
    "Name": "my-trail", 
    "TrailARN": "arn:aws:cloudtrail:us-east-2:123456789012:trail/my-trail", 
    "LogFileValidationEnabled": false, 
    "IsMultiRegionTrail": false, 
    "IsOrganizationTrail": false,
    "S3BucketName": "my-bucket"
}
```
To change a trail so that it logs global service events, use the `--include-global-service-events` option.

