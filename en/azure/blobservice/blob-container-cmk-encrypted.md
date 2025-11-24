[![CloudSploit](https://cloudsploit.com/img/logo-new-big-text-100.png "CloudSploit")](https://cloudsploit.com)

# AZURE / Blob Service / Blob Container CMK Encrypted

## Quick Info

| | |
|-|-|
| **Plugin Title** | Blob Container CMK Encrypted |
| **Cloud** | AZURE |
| **Category** | Blob Service |
| **Description** | Ensures that blob containers in storage account are CMK encrypted |
| **More Info** | Azure allows you to encrypt data in your blob containers using customer-managed keys (CMK) instead of using platform-managed keys, which are enabled by default. Configuring a customer-managed key for blob services ensures protection and control access to the key that encrypts your data. Customer-managed keys offer greater flexibility to manage access controls. |
| **AZURE Link** | https://learn.microsoft.com/en-us/azure/storage/common/customer-managed-keys-overview |
| **Recommended Action** | Ensure that all blob containers in storage account have CMK encryption enabled. |

## Important Note

**⚠️ This remediation guide applies only to new blob containers created after CMK encryption scope configuration. Encryption scopes are set at container creation time and cannot be changed for existing containers. To enable CMK encryption for existing containers, you must create new containers with CMK encryption scopes and migrate the data.**

## Detailed Remediation Steps

### Prerequisites

Before configuring CMK encryption for blob containers, ensure you have:
1. An Azure Key Vault with a key that will be used for encryption
2. The storage account must have appropriate permissions to access the Key Vault. The Key Vault must have an access policy that grants the storage account (or its managed identity) the following permissions: **Get**, **Unwrap Key**, and **Wrap Key**. If you see an "Access denied" message when selecting the key vault, you need to configure these permissions first.
3. The storage account must be configured to use customer-managed keys at the account level (optional but recommended)

### Step 1: Create an Encryption Scope with CMK

1. Log in to the Microsoft Azure Management Console.
2. Find the search bar at the top and search for **Storage account**. </br> <img src="/resources/azure/blobservice/blob-container-cmk-encrypted/step1.png"/>
3. Select the **Storage account** by clicking on the **Name** link to access the configuration changes.
4. In the left navigation panel, scroll down and click on **Encryption** under **Security + networking**. </br> <img src="/resources/azure/blobservice/blob-container-cmk-encrypted/step2.png"/>
5. On the **Encryption** page, click on the **Encryption scopes** tab (if not already selected), then click on the **+ Add** button at the top to create a new encryption scope.
6. In the **Create encryption scope** panel that opens on the right:
   - Enter a **Name** for the encryption scope in the **Encryption scope name** field (e.g., "cmk-encryption-scope")
   - Under **Encryption type**, select the radio button for **Customer-managed keys** (this should be selected by default)
   - Under **Encryption key**, select the radio button for **Select from key vault** </br> <img src="/resources/azure/blobservice/blob-container-cmk-encrypted/step3.png"/>
7. In the same **Create encryption scope** panel, configure the key vault settings:
   - **Subscription**: Select your subscription from the dropdown
   - **Key vault** (required): Click the dropdown and select your Key Vault from the list. If you see an access denied message, ensure the storage account has the necessary permissions (Get, Unwrap Key, Wrap Key) on the Key Vault.
   - **Key** (required): Click the dropdown and select the key from your Key Vault
   - **Infrastructure encryption**: Leave as **Disabled** (default) unless you require double encryption
8. Review all settings, then click the **Create** button at the bottom of the panel to save the encryption scope.
9. Wait for the encryption scope to be created successfully. You should see it listed on the **Encryption scopes** page with **Status** showing as **Enabled**.

### Step 2: Create New Blob Containers with CMK Encryption 

1. In the left navigation panel of your Storage account, click on **Containers** under **Data storage**. </br> <img src="/resources/azure/blobservice/blob-container-cmk-encrypted/step4.png"/>
2. Click on the **+ Container** button at the top to create a new container.
3. In the **New container** panel:
   - Enter a **Name** for the container
   - Select the **Public access level** (recommended: **Private (no anonymous access)**)
   - Under **Encryption scope**, select **Use a specific encryption scope**
   - In the **Encryption scope** dropdown, select the CMK encryption scope you created in Step 1
   - Click **Create**
4. The new container will be created with CMK encryption enabled. All blobs uploaded to this container will be encrypted using the customer-managed key from your Key Vault.

### Step 3: Verify CMK Encryption

1. Navigate back to the **Containers** page and select the container you just created.
2. In the container properties, verify that the **Default encryption scope** shows the CMK encryption scope name you configured.
3. Alternatively, you can verify by checking the encryption scopes:
   - Go to **Encryption** under **Security + networking**, then click on the **Encryption scopes** tab
   - Confirm that your encryption scope is listed with **Status** showing as **Enabled**
4. **Note**: You cannot change the encryption scope of an existing container. You must create a new container with CMK encryption. 
