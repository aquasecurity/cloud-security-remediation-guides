[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Resource Manager / Trusted Image Projects

## Quick Info

| | |
|-|-|
| **Plugin Title** | Trusted Image Projects |
| **Cloud** | GOOGLE |
| **Category** | Resource Manager |
| **Description** | Determine if \"Define Trusted Image Projects\" constraint policy is enforces at the GCP organization level. |
| **More Info** | Enforcing the \"Define Trusted Image Projects\" allows you to restrict disk image access and ensure that your project members can only create boot disks from trusted images. |
| **GOOGLE Link** | https://cloud.google.com/resource-manager/docs/organization-policy/org-policy-constraints |
| **Recommended Action** | Ensure that \"Define Trusted Image Projects\" constraint is enforced at the organization level. |

## Detailed Remediation Steps
1. Go to the Organization policies page.

    [Go to Organization policies](#https://console.cloud.google.com/iam-admin/orgpolicies/)

2. From the policies list, click Define trusted image projects. The Policy details page displays.

3. On the Policy details page, click Manage Policy. The Edit policy page displays.

4. On the Edit policy page, select Customize.

5. For Policy enforcement, select an enforcement option. For information about inheritance and the resource hierarchy, see Understanding Hierarchy Evaluation.

6. Click Add rule.

7. In the Policy values list, you can select whether this organization policy should allow access to all image projects, deny access to all image projects, or you can specify a custom set of projects to allow or deny access to.

    - To set the policy rule, complete one of the following options:

        - To allow users to create boot disks from all public images, select Allow All.

        - To restrict users from creating boot disk from all public images, select Deny All.

        - To specify a select set of public images that users can create boot disks from, select Custom. A Policy type and Custom values field displays.

            a. In the Policy type list, select Allow or Deny.

            b. In the Custom values field, enter the name of the image project using the projects/IMAGE_PROJECT format.

                - Replace IMAGE_PROJECT with the image project you want to set the constraint on.

                - You can add multiple image projects. For each image project that you want to add, click Add and enter the image project name.

8. To save the rule, click Done.

9. To save and apply the organization policy, click Save.

For more information, see [Setting up trusted image policies](#https://cloud.google.com/compute/docs/images/restricting-image-access)