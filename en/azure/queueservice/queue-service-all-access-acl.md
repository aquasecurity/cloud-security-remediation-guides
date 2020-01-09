[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Queue Service / Queue Service All Access ACL

## Quick Info

| | |
|-|-|
| **Plugin Title** | Queue Service All Access ACL |
| **Cloud** | AZURE |
| **Category** | Queue Service |
| **Description** | Ensures queues do not allow full write, delete, or read ACL permissions |
| **More Info** | Queues can be configured to allow object read, write or delete. This option should not be configured unless there is a strong business requirement. |
| **AZURE Link** | https://docs.microsoft.com/en-us/azure/storage/queues/storage-quickstart-queues-portal |
| **Recommended Action** | Disable global read, write, delete policies on all queues and ensure the ACL is configured with least privileges. |

## Detailed Remediation Steps

1. Log into the Microsoft Azure Management Console.
2. Select the "Search resources, services, and docs" option at the top and search for Storage account. </br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step3.png"/>
4. Click on the "Overveiw" in the selected "Storage account" and scroll down the right side of the settings and click on the "Queues" option under "Services".</br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step4.png"/>
5. Select the "Queue" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step5.png"/>
6. In the selected "Queue", click on the "Access Policy" and check the "Permissions" assosciated with the "Queue". If the "Queue" allows full write, delete, or read ACL permissions then the selected "Queue" is not as per the standard configurations.</br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step6.png"/>
7. Repeat steps number 2 - 6 to verify other "Queues" in the Azure account. </br>
8. Navigate to the "Storage accounts", select the "Storage account" and click on the "Name", select the "Overview" options and select the "Queue" by clicking on the "Name" as a link to access the configurations.</br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step8.png"/>
9. On the "Queue" configuration click on the "Access Policy" option and select the "Edit" option to make the changes.</br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step9.png"/>
10. Uncheck the global read/write/detele policies under the "Permissions" and click on the "OK" button to make the changes.</br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step10.png"/>
11. Click on the "Save" button at the top to save the configuration changes.</br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step11.png"/>
12. Repeat steps number 8 - 11 to ensures "Queues" do not allow full write, delete, or read ACL permissions.</br>
