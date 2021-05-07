<!-- markdownlint-disable MD002 MD041 -->

Prior to using Microsoft Graph Data Connect for the first time, you need to configure your Microsoft 365 tenant. This involves turning on the service and configuring a security group with permissions to approve data extraction requests.

## Grant Azure AD users the Global Administrator role

In this step, you will ensure that two users in your Microsoft 365 tenant have the Global Administrator role enabled.

1. Open a browser and go to your [Azure Portal](https://portal.azure.com/).

1. Sign in using an account with **Global Administrator** rights to your Azure and Microsoft 365 tenants.

1. On the sidebar navigation, select **Azure Active Directory (Azure AD)**.
  
    ![A screenshot showing the search results for Azure Active Directory in the Azure portal.](images/data-connect-aad.png)

1. On the Azure AD Overview page, select Users from the Manage section of the menu.
  
    ![A screenshot showing the manage section for users in the Azure Active Directory blade.](images/data-connect-aad-manage-users.png)

1. In the list of **All Users**, identify a user you will use in this tutorial that you have access to.

   1. Select the user by selecting their name.
   1. On the sidebar navigation menu, select **Assigned roles**.

        ![A screenshot showing the Azure AD Assigned roles for a specific user.](images/data-connect-aad-assigned-roles.png)

   1. If the role **Global Administrator** is not in the list of roles for the user.

        1. Select **Add assignment** button.
        1. Locate and select the **Global Administrator** role and then select the **Select** button.

   1. Repeat these steps with another user that you will use in this tutorial.

## Configure Microsoft Graph Data Connect consent request approver group

In this step, you will setup your Microsoft 365 tenant to enable usage of Microsoft Graph Data Connect.

1. Open a browser and go to your [Microsoft 365 Admin Portal](https://admin.microsoft.com/)

1. On the sidebar navigation, select **Active Groups**.
  
    ![A screenshot showing the active groups in the Microsoft 365 admin center.](images/data-connect-m365-act-grp.png)

1. Select the **Add a group** button.

1. Use the following to create the new **mail-enabled** security group and select the **Add** button.
   - **Type**: Mail-enabled security

    ![A screenshot showing a user selecting the mail-enabled security for a new group in the Microsoft 365 admin center.](images/data-connect-m365-mail-sec.png)

   - **Name**: Consent Request Approvers

    ![A screenshot showing a user is giving the group a name of "Consent Request Approvers" in the Microsoft 365 admin center.](images/data-connect-m365-cons-apprv.png)

   - **Email Prefix**: consentrequestapprovers

    ![A screenshot showing a user creating the email address for the previously created group in the Microsoft 365 admin center.](images/data-connect-m365-cons-apprv-pref.png)

1. **It can take up to an hour** before the newly created group shows up in the list. When the group has been created, select it.

    > [!IMPORTANT]
    > Change the View dropdown to **mail-enabled security** if you do not see Consent Request Approvers in the list of groups

1. On the **Members** section of the group dialog, select **Edit**.

1. Add the two users that you enabled the **Global Administrator** role to this new group.

## Enable Microsoft Graph Data Connect in your Microsoft 365 tenant

In this step, you will enable the Microsoft Graph Data Connect service on your Microsoft 365 tenant.

1. While you are still signed in to the Microsoft 365 Admin Portal, select the **Settings > Org settings** menu item.

1. Select the **Microsoft Graph Data Connect** service.

    ![A screenshot showing the "Services" in the "Org settings" blade. A user is toggling on the Microsoft Graph Data Connect service in the Microsoft 365 admin center.](images/data-connect-m365-mgdc-toggle.png)

1. Enable the toggle button at the top of the dialog to **turn Microsoft Graph Data Connect on or off for your entire organization**.

1. Enter **Consent Request Approvers** (or the name of the group you created previously) in the **group of users to make approval decisions** and select **Save**.
