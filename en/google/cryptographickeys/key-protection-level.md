[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# GOOGLE / Cryptographic Keys / Key Protection Level

## Quick Info

| | |
|-|-|
| **Plugin Title** | Key Protection Level |
| **Cloud** | GOOGLE |
| **Category** | Cryptographic Keys |
| **Description** | Ensure that cryptographic keys have protection level equal to or above desired protection level. |
| **More Info** | Cloud KMS cryptographic keys should be created with protection level set by your organization's compliance and security rules. |
| **GOOGLE Link** | https://cloud.google.com/kms/docs/reference/rest/v1/ProtectionLevel |
| **Recommended Action** | Create cryptographic keys according to desired protection level. |

## Detailed Remediation Steps
1. In the Google Cloud console, go to the Key Management page. 

2. Click the name of the key ring for which you will create a key.

3. Click Create key.

4. For Key name, enter a name for your key.

5. For Protection level, select Software or HSM.

6. For Key material, select Generated key.

7. For Purpose, select either Symmetric encrypt/decrypt or Asymmetric decrypt.

    a. If selecting Symmetric encrypt/decrypt:

        i. Accept the default values for Rotation period and Starting on.

    b. If selecting Asymmetric decrypt:

        i. For Algorithm, select 3072 bit RSA - OAEP Padding - SHA256 Digest. You can change this value on future key versions.

8. Click Create.