[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Kubernetes / Cluster Encryption Enabled

## Quick Info

| | |
|-|-|
| **Plugin Title** | Cluster Encryption Enabled |
| **Cloud** | GOOGLE |
| **Category** | Kubernetes |
| **Description** | Ensure that GKE clusters have KMS encryption enabled to encrypt application-layer secrets. |
| **More Info** | Application-layer secrets encryption adds additional security layer to sensitive data such as Kubernetes secrets stored in etcd. |
| **GOOGLE Link** | https://cloud.google.com/kubernetes-engine/docs/how-to/encrypting-secrets |
| **Recommended Action** | Ensure that all GKE clusters have the desired application-layer secrets encryption level. |

## Detailed Remediation Steps
1. Log into the Google Cloud Platform Console.
2. Scroll down the left navigation panel and choose the "Kubernetes Engine" then select the "Clusters". </br> <img src="/resources/google/kubernetes/cluster-encryption-enabled/step2.png"/>
3. On the "Kubernetes clusters" page , click on the "Name" of the cluster you want to modify.</br> <img src="/resources/google/kubernetes/cluster-encryption-enabled/step3.png"/>
4. Under Security, in the Application-layer secrets encryption field, click Edit Application-layer secrets encryption. </br><img src="/resources/google/kubernetes/cluster-encryption-enabled/step4.png"/>
5. Select the Enable Application-layer secrets encryption checkbox and choose the KMS key. To Create a Cloud KMS key refer to https://cloud.google.com/kubernetes-engine/docs/how-to/encrypting-secrets#creating-key. </br><img src="/resources/google/kubernetes/cluster-encryption-enabled/step5.png"/>
6. Click Save Changes. </br>
7. Repeat steps number 3 - 6 to enable application-layer secrets encryption for other "Clusters" in the account.</br>