[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / EC2 / Unused Amazon Machine Images

## Quick Info

| | |
|-|-|
| **Plugin Title** | Unused Amazon Machine Images |
| **Cloud** | AWS |
| **Category** | EC2 |
| **Description** | Ensures that all Amazon Machine Images are in use to ensure cost optimization |
| **More Info** | All unused/deregistered Amazon Machine Images should be deleted to avoid extraneous cost |
| **AWS Link** | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/deregister-ami.html |
| **Recommended Action** | Delete the unused/deregistered AMIs |

## Detailed Remediation Steps
The procedure that you'll use to clean up your AMI depends on whether it's backed by Amazon EBS or instance store. For more information, see https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ComponentsAMIs.html#display-ami-root-device-type. </br>
To clean up your Amazon EBS-backed AMI. </br>
1. Log into the AWS Management Console. </br>
2. Select the "Services" option and search for EC2. </br> 
3. In the navigation pane, choose AMIs. </br>
4.Select the AMI to deregister, and take note of its ID—this can help you find the snapshots to delete in the next step.</br>
5. Choose Actions, Deregister AMI. When prompted for confirmation, choose Deregister AMI. </br>
Note:
It might take a few minutes before the console removes the AMI from the list. Choose Refresh to refresh the status. </br>
Delete snapshots that are no longer needed. </br>
1. In the navigation pane, choose Snapshots. </br>
2. Select a snapshot to delete (look for the AMI ID from the prior step in the Description column).</br>
3. Choose Actions, Delete snapshot. When prompted for confirmation, choose Delete. </br>

(Optional) Terminate instances </br>
1. If you are finished with an instance that you launched from the AMI, you can terminate it. </br>
2. In the navigation pane, choose Instances, and then select the instance to terminate. </br>
3. Choose Instance state, Terminate instance. When prompted for confirmation, choose Terminate.</br>

Clean up your instance store-backed AMI </br>
1. Deregister the AMI using the deregister-image command as follows. </br>
aws ec2 deregister-image --image-id ami_id </br>
2. Delete the bundle in Amazon S3 using the ec2-delete-bundle (AMI tools) command as follows. </br>
ec2-delete-bundle -b myawsbucket/myami -a your_access_key_id -s your_secret_access_key -p image </br>
3. (Optional) If you are finished with an instance that you launched from the AMI, you can terminate it using the terminate-instances command as follows. </br>
aws ec2 terminate-instances --instance-ids instance_id </br>
4. (Optional) If you are finished with the Amazon S3 bucket that you uploaded the bundle to, you can delete the bucket. To delete an Amazon S3 bucket, open the Amazon S3 console, select the bucket, choose Actions, and then choose Delete. </br>