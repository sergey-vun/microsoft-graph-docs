<!-- markdownlint-disable MD002 MD041 -->

The next step is to use the Azure Data Factory to create a pipeline to extract the data from Microsoft 365 to the Azure Storage account using Microsoft Graph data connect.

## Create an Azure Data Factory pipeline

1. Open a browser and go to your [Azure Portal](https://portal.azure.com/).

1. Sign in using an account with **Global Administrator** rights to your Azure and Microsoft 365 tenants.

    > [!NOTE]
    > Keep track of the user you are using in this step as you will need to switch to the other user you granted the **Global Administrator** role and that has multi-factor authentication enabled on their account in a later step.

1. On the sidebar navigation, select **Create a resource**.

1. Find the **Data Factory** resource type and use the following values to create it, then select **Create**.

    1. **Name**: dfM365toBlobStorage
    2. **Subscription**: select your Azure subscription
    3. **Resource group**: GraphDataConnect
    4. **Version**: V2
    5. **Location**: pick an Azure region in the same region as your Microsoft 365 region

    ![A screenshot showing the successful creation of the new Azure Data Factory service in the Azure portal.](images/data-connect-adf-create.png)

1. After the Azure Data Factory resource is created, select the **Author and Monitor** tile to launch the Azure Data Factory full screen editor.

    ![A screenshot showing the Azure Portal UI for the Data Factory service. The user is clicking the Author and Monitor button.](images/data-connect-adf-auth-and-mon.png)

1. Switch from the **Overview** to the **Manage** experience by selecting it from the left-hand navigation.

1. **Optional step**. By default, the Azure Data Factory will use an integration runtime that is auto-resolving the region. Because Data Connect requires that your source and destination, and integration runtime to exist in the same Microsoft 365 region, we recommend that you create a new integration runtime with a fixed region.

    1. Select **Integration runtimes** > **New**.
    1. Select **Azure, Self-Hosted** and select **Continue**.
    1. Select **Azure** for network environment and select **Continue**.

    ![A screenshot showing the Azure Portal UI for the Data Factory service. The user is selecting the Azure option for the network environment.](images/data-connect-adf-network.png)

    1. Use the following details to complete the form on the final screen and then select **Create**.

        - **Name**: name of your integration runtime
        - **Description**: enter a description
        - **Region**: select the region that matches your Microsoft 365 region

1. Switch from the **Manage** to the **Author** experience by selecting it from the left-hand navigation and create a new pipeline by selecting the **plus** icon, then **pipeline**.

    ![A screenshot showing the Azure portal UI for the Data Factory service. The user is creating a new pipeline.](images/data-connect-adf-pipeline-create.png)

    - Drag the **Copy Data** activity from the **Move and Transform** section onto the design surface.

    ![A screenshot showing the Azure portal UI for the Data Factory service. The user is dragging the copy data activity into the editor on the right side of the screen.](images/data-connect-adf-pipeline-copy-data.png)

    - Select the activity in the designer.
    - In the activity editor pane below the designer, select the **Source** tab, then select **New**.
    - Locate the dataset **Office 365**, select it and then select the **Continue** button.

    ![A screenshot showing the Azure portal UI for the Data Factory service. The user is selecting the Office 365 dataset in the UI and selecting the continue button afterwards.](images/data-connect-adf-pipeline-dataset.png)

    - The designer will create a new tab for the Microsoft 365 connector. Select the **Connection** tab in the connector's editor, then the **New** button.
    - In the dialog that appears, enter the previously created Azure AD application's **Application ID** and **Password** in the **Service principal ID** and **Service principal key** fields, then select **Finish**.

    > [!TIP]
    > If you created a dedicated integration runtime, select it in the **Connect via integration runtime** dropdown.

    ![A screenshot showing the Azure portal UI for the Data Factory service. The user is configuring the integration runtime with the service principal key.](images/data-connect-adf-linked-service.png)

    - After creating the Microsoft 365 connection, for the **Table** field, select **BasicDataSet_v0.Message_v0**.
    - Switch from **Office365Table** to **Pipeline > Source**. Use the following values for the **Date filter**.

        - **Column name**: CreatedDateTime
        - **Start time (UTC)**: select a date sometime prior to the current date
        - **End time (UTC)**: select the current date

    - Select the **Source** tab and then select **Import schema**.
    - With the source configured for your **copy data** activity, now configure the **sink**, or the location where data will be stored.
    - Select the tab in the designer for your pipeline.
    - Select the **copy data** activity, then select the sink tab.
    - Select the **New** button, select **Azure Blob Storage**, and then select the **Continue** button.
    - Select **Binary** as the format for the data and then select the **Continue** button.
    - Give the dataset the name **M365JsonFile** and create new linked service if it does not exist already.
    - Select the **Connection** tab, then select **New**.
    - Set the following values in the dialog, then select **Finish**.

        - **Authentication method**: Service principal
        - **Azure subscription**: Select all
        - **Storage account name**: {tenantid}gdcdump
        This is the storage account created earlier in this exercise.
        - **Tenant**: enter the ID of your Azure tenant
        - **Service principal ID**: enter the ID of the Azure AD application you previously created
        - **Service principal key**: enter the hashed key of the Azure AD application you previously created

        > [!NOTE]
        > If you created a dedicated integration runtime, select it in the Connect via integration runtime dropdown.

        ![A screenshot showing the Azure portal UI for the Data Factory service. The user is finishing configuring the Data Factory linked service settings for Azure Blob Storage.](images/data-connect-adf-ls-config.png)

    - Next to the **File path** field, select **Browse**.
    - Select the name of the storage container you created previously.

      ![A screenshot showing the Azure portal UI for the Data Factory service. The user is configuring the container and file path in the sink properties.](images/data-connect-adf-sa-fp-config.png)

    - Ensure that the **File format** is set to **Binary** format.
    - Set the **File pattern** to **Set of objects**.

1. With the pipeline created, select the **Validate All** button at the top of the designer.

1. After validating (and fixing any issues that were found), select the **Publish All** button at the top of the designer.

## Run the Azure Data Factory Pipeline

With the pipeline created, now it is time to run it.

> [!NOTE]
> It can take several minutes for the consent request to appear and it is not uncommon for the entire process (start, requesting consent and after approving the consent completing the pipeline run) to take over 40 minutes.

1. In the Azure Data Factory designer, with the pipeline open, select **Add trigger > Trigger Now**.

    ![A screenshot showing the Azure portal UI for the Data Factory service to show how to activate a trigger in the pipeline.](images/data-connect-adf-run-trigger.png)

1. After starting the job, from the sidebar menu, select **Monitor** to view current running jobs.

1. Locate the pipeline run you just started in the list. In the **Actions** column, select the **View Activity Runs** icon.

1. On the **Activity Runs** screen, you will see a list of all the activities that are running in this pipeline. Our pipeline only has one activity that should show as currently In Progress.

1. While the status might show as In Progress, the request might be paused internally as the request for access to the data in Microsoft 365 might need to be approved. You can see if this is the case by selecting the **Details** icon in the **Actions** column.

1. In the **Details** screen, look for the status of the pipeline activity as highlighted in the following image. In this case you can see it is in a state of **RequestingConsent**.

    ![A screenshot showing the Azure portal UI for the Data Factory service where the request's load status is set to "RequestingConsent".](images/data-connect-adf-wait-for-approval.png)

1. At this point, the activity run is internally paused until someone manually approves the consent request.
