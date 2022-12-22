[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AWS / Lambda / Lambda Environment Variables Client Side Encryption

## Quick Info

| | |
|-|-|
| **Plugin Title** | Lambda Environment Variables Client Side Encryption |
| **Cloud** | AWS |
| **Category** | Lambda |
| **Description** | Ensure that all sensitive AWS Lambda environment variable values are client side encrypted. |
| **More Info** | AWS Lambda lets you encrypt environment variable values prior to sending them to Lambda. Environment variables are often used to store sensitive information such as passwords. Such variable valuesshould be encrypted for security best practices. |
| **AWS Link** | https://docs.aws.amazon.com/lambda/latest/dg/configuration-envvars.html |
| **Recommended Action** | Encrypt environment variables that store sensitive information. |

## Detailed Remediation Steps

1. Use the AWS Key Management Service (AWS KMS) to create any customer managed keys for Lambda to use for server-side and client-side encryption. For more information, see https://docs.aws.amazon.com/kms/latest/developerguide/create-keys.html. </br>
2. Using the Lambda console, navigate to the Edit environment variables page. </br>
a. Open the Functions page of the Lambda console. </br>
b. Choose a function. </br>
c. Choose Configuration, then choose Environment variables from the left navigation bar. </br>
d. In the Environment variables section, choose Edit. </br>
e. Expand Encryption configuration. </br>
3. Optionally, enable console encryption helpers to use client-side encryption to protect your data in transit. </br>
a. Under Encryption in transit, choose Enable helpers for encryption in transit. </br>
b. For each environment variable that you want to enable console encryption helpers for, choose Encrypt next to the environment variable. </br>
c. Under AWS KMS key to encrypt in transit, choose a customer managed key that you created at the beginning of this procedure. </br>
d. Choose Execution role policy and copy the policy. This policy grants permission to your function's execution role to decrypt the environment variables. Save this policy to use in the last step of this procedure. </br>
e. Add code to your function that decrypts the environment variables. Choose Decrypt secrets snippet to see an example. </br>
4. Optionally, specify your customer managed key for encryption at rest. </br>
a. Choose Use a customer master key. </br>
b. Choose a customer managed key that you created at the beginning of this procedure. </br>
5. Choose Save. </br>
6. Set up permissions. If you're using a customer managed key with server-side encryption, grant permissions to any AWS Identity and Access Management (IAM) users or roles that you want to be able to view or manange environment variables on the function. For more information, see https://docs.aws.amazon.com/lambda/latest/dg/configuration-envvars.html#managing-permissions-to-your-server-side-encryption-key. If you're enabling client-side encryption for security in transit, your function needs permission to call the kms:Decrypt API operation. Add the policy that you saved previously in this procedure to the function's execution role https://docs.aws.amazon.com/lambda/latest/dg/lambda-intro-execution-role.html. </br>