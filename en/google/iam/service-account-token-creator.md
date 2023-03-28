[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Compute / Service Account Token Creator

## Quick Info

| | |
|-|-|
| **Plugin Title** | Service Account Token Creator |
| **Cloud** | GOOGLE |
| **Category** | Compute |
| **Description** | Ensures that no users have the Service Account Token Creator role. |
| **More Info** | For best security practices, IAM users should not have Service Account Token Creator role. |
| **GOOGLE Link** | https://cloud.google.com/compute/docs/disks |
| **Recommended Action** | Ensure that no IAM user have Service Account Token Creator Role at GCP project level.|

## Detailed Remediation Steps
1.  In the Google Cloud console, go to the IAM page.

    [Go to IAM](https://console.cloud.google.com/projectselector/iam-admin/iam?supportedpurview=project,folder,organizationId)

2.  Select a project, folder, or organization (in this case the GCP project).

    The Google Cloud console lists all the principals who have been granted roles on your project, folder, or organization. This list includes principals who have inherited roles on the resource from parent resources. For more information about policy inheritance, see [Policy inheritance and the resource hierarchy](https://cloud.google.com/iam/docs/policies#inheritance).
Check to see if any have the Service Account Access Role.

3.  Optional: To view role grants for [Google-managed service accounts](https://cloud.google.com/iam/docs/service-account-types#google-managed), select the Include Google-provided role grants checkbox.