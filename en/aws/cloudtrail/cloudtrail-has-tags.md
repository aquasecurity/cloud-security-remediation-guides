[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / CloudTrail / CloudTrail Has Tags

## Quick Info

| | |
|-|-|
| **Plugin Title** | CloudTrail Has Tags |
| **Cloud** | AWS |
| **Category** | CloudTrail |
| **Description** |Ensure that Cloudtrail have tags |
| **More Info** | Tags help you to group resources together that are related to or associated with each other. It is a best practice to tag cloud resources to better organize and gain visibility into their usage. |
| **AWS Link** | https://docs.aws.amazon.com/awscloudtrail/latest/APIReference/API_AddTags.html |
| **Recommended Action** | Modify cloud trail and add tags |
    
## Detailed Remediation Steps
1. Log into the AWS Management Console.
2. Select the "Services" option and search for "CloudTrail".</br><img src="/resources/aws/cloudtrail/cloudtrail-has-tags/step2.png"/>
3. In the "Dashboard" panel in Trails section select "trail" that needs to have tags under "Name" column.</br> <img src="/resources/aws/cloudtrail/cloudtrail-has-tags/step3.png"/>
4. On trail details page scroll down to "Tags" section and Click on "Manage Tags" button.</br><img src="/resources/aws/cloudtrail/cloudtrail-has-tags/step4.png"/>
5. On the edit tags page Click on "Add Tag" button and enter the key-value pair for tag in text boxes and Click "Save Changes" button.</br><img src="/resources/aws/cloudtrail/cloudtrail-has-tags/step5.png"/>
