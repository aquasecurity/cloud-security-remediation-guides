[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Network Security Groups / Default Security Group

## Quick Info

| | |
|-|-|
| **Plugin Title** | Default Security Group |
| **Cloud** | AZURE |
| **Category** | Network Security Groups |
| **Description** | Ensures that default security groups block all traffic by default |
| **More Info** | The default security group is often used for resources launched without a defined security group. For this reason, the default rules should be set to block all traffic to prevent an accidental exposure. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/virtual-network/manage-network-security-group |
| **Recommended Action** | Update the rules for the default security group to deny all traffic by default |

## Detailed Remediation Steps

1. Log in to the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Network security groups. </br> <img src="/resources/azure/networksecuritygroups/default-security-group/step2.png"/>
3. Select the "Network security group" that needs to be verified and click on its "Name". </br> <img src="/resources/azure/networksecuritygroups/default-security-group/step3.png"/>
4. Scroll down the left navigation panel and select the "Inbound security rules" under "Settings." </br> <img src="/resources/azure/networksecuritygroups/default-security-group/step4.png"/>
5. Under the "Inbound security rules" check "Name" "DenyAllInBound" is present and traffic status is set to "Deny" under "Action" column. If it is not present, then the selected "Default security group" is not as per the best practices recommended by Azure.</br> <img src="/resources/azure/networksecuritygroups/default-security-group/step5.png"/>
6. Repeat step number 5 for the "Outbound security rules" as well. </br> <img src="/resources/azure/networksecuritygroups/default-security-group/step6.png"/>
7. Navigate to the "Network security group" and select the security group that needs to be modified to deny all traffic by default.</br> <img src="/resources/azure/networksecuritygroups/default-security-group/step8.png"/>
8. Scroll down the left navigation panel and choose "Inbound security rules" under "Settings."</br> <img src="/resources/azure/networksecuritygroups/default-security-group/step9.png"/>
9. Select the protocol which is having traffic access by default and then click on the delete option on extreme right or top to remove the specific protocol.</br> <img src="/resources/azure/networksecuritygroups/default-security-group/step10.png"/>
10. In the "Delete security rule" dialouge box select "Yes". </br> <img src="/resources/azure/networksecuritygroups/default-security-group/step10.png"/>
11. Repeat step number 9 & 10 for "Outbound security rules."</br> <img src="/resources/azure/networksecuritygroups/default-security-group/step11.png"/>
12. Repeat steps number 7 - 11 to update the rules for the default security group to deny all traffic by default.</br>
