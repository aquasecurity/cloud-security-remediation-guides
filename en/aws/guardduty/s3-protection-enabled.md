# AWS / GuardDuty / S3 GuardDuty Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | S3 GuardDuty Enabled |
| **Cloud** | AWS |
| **Category** | GuardDuty |
| **Description** | Ensures GuardDuty is enabled for S3 buckets. |
| **More Info** | Enabling GuardDuty S3 protection helps to detect and prevent unauthorized access to your S3 buckets. |
| **AWS Link** | https://docs.aws.amazon.com/guardduty/latest/ug/s3-protection.html |
| **Recommended Action** | Enable GuardDuty S3 protection for all AWS accounts. |

## Detailed Remediation Steps
**Note**
You can enable S3 Protection in an account in any Region where GuardDuty [supports this feature](https://docs.aws.amazon.com/guardduty/latest/ug/guardduty_regions.html). 

When you enable GuardDuty in an AWS account in a new Region your account in this Region will start incurring usage cost. For more information, see [Estimating GuardDuty usage cost](https://docs.aws.amazon.com/guardduty/latest/ug/monitoring_costs.html).

**Enabling S3 Protection for a standalone account**
1. Sign in to the AWS Management Console and open the GuardDuty [console]( https://console.aws.amazon.com/guardduty/).

2. From the Region selector in the upper-right corner, select a Region where you want to enable S3 Protection.

3. In the navigation pane, choose S3 Protection.

4. The S3 Protection page provides the current status of S3 Protection for your account. Choose Enable or Disable to enable or disable S3 Protection at any point in time.

5. Choose Confirm to confirm your selection.
6. To enable S3 Protection in multiple-account environments see https://docs.aws.amazon.com/guardduty/latest/ug/s3-multiaccount.html.