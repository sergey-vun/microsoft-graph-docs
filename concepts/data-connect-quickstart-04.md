<!-- markdownlint-disable MD002 MD041 -->

In this step you will create an Azure Storage account where Microsoft Graph data connect will store the data extracted from Office 365 for further processing.

1. Open a browser and navigate to your [Azure Portal](https://portal.azure.com/).

1. Login using an account with **Global Administrator** rights to your Azure and Office 365 tenants.

1. Select **Create a resource** from the sidebar navigation.

    ![Azure-Storage-Create](images/data-connect-azure-storage-create.png)

1. Find the **Storage Account** resource type and use the following values to create it, then select **Review + create**:

    - **Subscription**: select your Azure subscription
    - **Resource group**: GraphDataConnect (or select an existing resource group)
    - **Storage account name**: mgdcm365datastore
    - **Location**: pick an Azure region in the same region as your Office 365 region
    - **Performance**: Standard
    - **Account kind**: StorageV2 (general purpose v2)
    - **Replication**: Read-access geo-redundant storage (RA-GRS)
    - **Access tier**: Hot

1. Review that the settings match those shown in the previous step and select **Create**.

    ![Azure-Storage-Review](images/data-connect-azure-storage-review.png)

1. Once the Azure Storage account has been created, grant the Azure AD application previously created the proper access to it.

    1. Select the **Azure Storage account**.
    1. In the sidebar menu, select **Access control (IAM)**.

        ![Azure-Storage-IAM](images/data-connect-azure-storage-iam.png)

    1. Select the **Add** button in the **Add a role assignment** block.
    1. Use the following values to find the application you previously selected to grant it the **Storage Blob Data Contributor** role, then select **Save**:

        - **Role**: Storage Blob Data Contributor
        - **Assign access to**: Azure AD user, group or service principal
        - **Select**: Microsoft Graph data connect Data Transfer (the name of the Azure AD application you created previously)

        ![Azure-Storage-Role](images/data-connect-azure-storage-role.png)

1. Create a new container in the **mgdcm365datastore** Azure Storage account:

    1. Select the **mgdcm365datastore** Azure Storage account.
    1. In the sidebar menu, select **Containers** under the **Blob** service section.
    1. Select the **+Container** button at the top of the page and use the following values and then select **Create**:

        - **Name**: m365mails
        - **Public access level**: Private (no anonymous access)

        ![Azure-Storage-Container](images/data-connect-azure-storage-container.png)
