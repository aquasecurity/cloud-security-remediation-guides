[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudTrail / CloudTrail Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudTrail Enabled |
| **Cloud** | AWS |
| **Category** | CloudTrail |
| **Description** | Ensures CloudTrail is enabled for all regions within an account |
| **More Info** | CloudTrail should be enabled for all regions in order to detect suspicious activity in regions that are not typically used. |
| **AWS Link** | http://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-getting-started.html |
| **Recommended Action** | Enable CloudTrail for all regions and ensure that at least one region monitors global service events |

## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "CloudTrail".</br>![Step 2](/resources/aws/cloudtrail/cloudtrail-enabled/step2.png "Step 2 - Services")
3. In the "Dashboard" panel click on "View trails" button.</br> ![Step 3](/resources/aws/cloudtrail/cloudtrail-enabled/step3.png "Step 3 - Trails")
4. Select the "trail" that needs to be verified under "Name" column.</br>![Step 4](/resources/aws/cloudtrail/cloudtrail-enabled/step4.png "Step 4 - Name")
5. Click the pencil icon to go into "Trail Settings" and verify the checkbox marked against "Apply trail to all regions
". If "No" is selected than create and manage a trail across all regions is not possible.</br>![Step 5](/resources/aws/cloudtrail/cloudtrail-enabled/step5.png "Step 5 - Trail Settings")
6. Go to "Trail Settings" and click on "Yes" checkbox to enable the "Apply trail to all regions" which receive the log files containing event history for the new region without taking any action. Click on the "Save" button to make the changes. </br>![Step 6](/resources/aws/cloudtrail/cloudtrail-enabled/step6.png "Step 6 - Apply trail")
7. Scroll down and go to "Additional Configuration" settings and click on the pencil icon to make the changes.</br>![Step 7](/resources/aws/cloudtrail/cloudtrail-enabled/step7.png "Step 4 - Additional Configuration")
8. Click on the "Yes" checkbox corresponding to the "Include global services" and click on "Save" button to make the changes.</br>![Step 8](/resources/aws/cloudtrail/cloudtrail-enabled/step8.png "Step 8 - Global Services")
9. CloudTrail is enabled for all regions with global service events now.</br>
