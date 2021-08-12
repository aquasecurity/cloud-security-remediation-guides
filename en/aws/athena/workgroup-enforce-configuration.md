[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Athena / Workgroup Enforce Configuration

## Quick Info

| | |
|-|-|
| **Plugin Title** | Workgroup Enforce Configuration |
| **Cloud** | AWS |
| **Category** | Athena |
| **Description** | Ensures Athena workgroups do not allow clients to override configuration options. |
| **More Info** | Athena workgroups support the ability for clients to override configuration options, including encryption requirements. This setting should be disabled to enforce encryption mandates. |
| **AWS Link** | https://docs.aws.amazon.com/athena/latest/ug/workgroups-settings.html |
| **Recommended Action** | Disable the ability for clients to override Athena workgroup configuration options. |

## Detailed Remediation Steps
1. Log in to the AWS Management Console.
2. Select the "Services" option and search for Athena. </br> <img src="/resources/aws/athena/workgroup-enforce-configuration/step2.png"/>
3. On the "Athena" dashboard, choose the "Workgroup: Primary" option at the top right console.</br> <img src="/resources/aws/athena/workgroup-enforce-configuration/step3.png"/>
4. On the "Workgroups" page, select the radio button near the "Name" and click on the "View Details" option.</br> <img src="/resources/aws/athena/workgroup-enforce-configuration/step4.png"/>
5. On the "Workgroup: primary" page, if the "Override client-side settings" is diabled under the "Overview" tab then the selected Athena workgroups allow clients to override configuration options.</br> <img src="/resources/aws/athena/workgroup-enforce-configuration/step5.png"/>
6. Repeat steps number 2 - 5 to check other Athena Workgroups in the account.</br>
7. Navigate to the Athena console using the link https://console.aws.amazon.com/athena/ .</br> <img src="/resources/aws/athena/workgroup-enforce-configuration/step7.png"/>
8. On the "Athena Console", click on the "Workgroup: primary" option at the top right and in the "View details" tab under the Workgroups after selecting the workgroup.  </br> <img src="/resources/aws/athena/workgroup-enforce-configuration/step8.png"/>
9. Click on the "Edit Workgroup" option at the top.</br> <img src="/resources/aws/athena/workgroup-enforce-configuration/step9.png"/>
10. On the "Edit workgroup" page, scroll down and click the checkbox next to the "Override client-side settings" under the Settings tab.</br> <img src="/resources/aws/athena/workgroup-enforce-configuration/step10.png"/>
11. Click on the "Save" button at the bottom to make the changes.</br> <img src="/resources/aws/athena/workgroup-enforce-configuration/step11.png"/>
12. Repeat steps number 7 - 11 to disable the ability for clients to override Athena workgroup configuration options.</br>


