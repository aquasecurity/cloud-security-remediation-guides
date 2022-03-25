[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Network Security Groups / Excessive Security Groups

## Quick Info

| | |
|-|-|
| **Plugin Title** | Excessive Security Groups |
| **Cloud** | AZURE |
| **Category** | Network Security Groups |
| **Description** | Determines if there are an excessive number of security groups in the account |
| **More Info** | Keeping the number of security groups to a minimum helps reduce the attack surface of an account. Rather than creating new groups with the same rules for each project, common rules should be grouped under the same security groups. For example, instead of adding port 22 from a known IP to every group, create a single "SSH" security group which can be used on multiple instances. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-network/manage-network-security-group |
| **Recommended Action** | Limit the number of security groups to prevent accidental authorizations. |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Network security groups. </br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step2.png"/>
3. Verify the number of Security Groups which are having the same security rules and used separately. </br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step3.png"/>
4. Click on the "Name" of the selected "Network security group" to access the port configurations. </br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step4.png"/>
5. In the "Overview" tab scroll down the page and check the "Inbound security rules." </br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step5.png"/>
6. Copy the Inbound and Outbound "security rules" which are in common in both the security groups.</br>
7. Repeat steps number 2 - 6 to verify other "Security Groups" in the account.</br>
8. Navigate to the "Network security groups" and click on the "Create" button at the top to add new security groups having common security rules.</br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step8.png"/>
9. On the "Create a network security group" page enter the details Resource Group, Name, Details and click on the "Review+Create" button to make the changes.</br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step9.png"/>
10. On the Review page, click on the "Create" button to proceed. </br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step10.png"/>
11. Click on the newly created "Network Security Group" and select the "Inbound security rules" under Security.</br>  <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step11.png"/>
12. Click on the "Add" button at the top and paste the rules copied in Step 6. </br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step12.png"/>
13. Once the new security group has all the same rules, navigate to the "Resources" using those Security Groups and change the groups accordingly.</br>
14. Navigate to "Network Security Groups" and  select the old "Security Groups" by clicking on its name and delete it by clicking "Delete" at the top of the page to prevent accidental authorizations.</br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step14.png"/>
15. In the "Delete network security group" dialougue box click "Yes" to finish deletion process..</br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step15.png"/>
16. Repeat steps number 8 - 15 to limit the number of security groups to prevent accidental authorizations.</br>

