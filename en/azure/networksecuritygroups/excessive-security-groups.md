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

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Network security groups. </br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step2.png"/>
3. Verify the number of Security Groups which are having the same security rules and used separately. </br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step3.png"/>
4. Click on the "Name" of the selected "Network security group" to access the port configurations. </br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step4.png"/>
5. In the "Overview" tab scroll down the page and check the "Inbound security rules." </br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step5.png"/>
6. Copy the Inbound and Outbound "security rules" which are in common in both the security groups.</br>
7. Repeat steps number 2 - 6 to verify other "Security Groups" in the account.</br>
8. Navigate to the "Network security group" and click on the "Add" button at the top to add new security groups having common security rules.</br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step8.png"/>
9. On the "Create a network security group" page enter the details Resource Group, Name, Details and click on the "Review+Create" button to make the changes.</br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step9.png"/>
10. Click on the newly created "Network Security Group" and select the "Inbound security rules" under Security.</br>  <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step10.png"/>
11. Click on the "Add" button at the top and paste the rules copied in Step 6. </br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step11.png"/>
12. Once the new security group has all the same rules, navigate to the "Resources" using those Security Groups and change the groups accordingly.</br>
13. Navigate to "Network Security Group" and delete the old "Security Groups" to prevent accidental authorizations.</br> <img src="/resources/azure/networksecuritygroups/excessive-security-groups/step13.png"/>
14. Repeat steps number 8 - 13 to limit the number of security groups to prevent accidental authorizations.</br>

