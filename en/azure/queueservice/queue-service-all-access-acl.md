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
2. In the search bar at the top search for Storage and select "Storage accounts" from the result. </br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step2.png"/>
3. Select the "Storage account" by clicking on the "Name" link to access the configuration changes. </br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step3.png"/>
4. In the left navigation panel, scroll down and click on the "Queues" option under "Data storage".</br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step4.png"/>
5. Select the "Queue" by clicking on the triple dot (...) at the end of the row and click "Access policy". </br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step5.png"/>
6. On the "Access Policy" pane check the "Permissions" assosciated with the "Queue". If it says "raup" then the queue allows full write, delete, or read ACL permissions and is not as per the security recommendations.</br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step6.png"/>
7. Click the triple dot (...) and click "Edit" option to make changes.</br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step7.png"/>
8. In the "Edit policy" popup that opens, click the "Permissions" dropdown, uncheck the global read and update policies then click on the "OK" button to save the changes.</br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step8.png"/>
9. Click on the "Save" button at the top to save the configuration changes.</br> <img src="/resources/azure/queueservice/queue-service-all-access-acl/step9.png"/>
12. Repeat steps number 8 - 11 to ensures "Queues" do not allow full write, delete, or read ACL permissions.</br>
