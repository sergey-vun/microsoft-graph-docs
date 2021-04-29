---
title: Microsoft Graph Data Connect quickstart
description: A quick start guide for Microsoft Graph Data Connect.
author: fercobo-msft
ms.author: fercobo
localization_priority: Priority
ms.prod: data-connect
ms.topic: quickstart
ms.date: 04/28/2021
ms.custom: template-quickstart
---

# Setup your Office 365 tenant and enable Microsoft Graph Data Connect

Prior to using Microsoft Graph Data Connect for the first time, you need to configure your Office 365 tenant. This involves turning on the service and configuring a security group with permissions to approve data extraction requests.

## Grant Azure AD users the Global Administrator role

In this step you will ensure that two users in your Office 365 tenant have the Global Administrator role enabled.

1. Open a browser and navigate to your [Azure Portal](https://portal.azure.com/).
2. Login using an account with **Global Administrator** rights to your Azure and Office 365 tenants.
3. Select Azure Active Directory (Azure AD) from the sidebar navigation or using the search bar:
![AAD](images/data-connect-aad.png)
4. On the Azure AD Overview page, select Users from the Manage section of the menu:
![AAD-manage-users](images/data-connect-aad-manage-users.png)
5. In the list of **All Users**, identify a user you will use in this lab that you have access to.

   1. Select the user by selecting their name.
   1. In the sidebar navigation menu, select **Assigned roles**.
    ![AAD-assigned-roles](images/data-connect-aad-assigned-roles.png)
   1. If the role **Global Administrator** is not in the list of roles for the user:
     - Select **Add assignment** button.
     - Locate and select the **Global Administrator** role and then select the **Select** button.
   1. Repeat these steps with another user that you will use in this lab.

## Configure Microsoft Graph Data Connect consent request approver group

In this step you will setup your Office 365 tenant to enable usage of Microsoft Graph Data Connect.

1. Open a browser and navigate to your [Microsoft 365 Admin Portal](https://admin.microsoft.com/)
2. In the sidebar navigation, select **Active Groups**.
![M365-ADM-Portal-Active-Groups](images/data-connect-m365-act-grp.png)
3. Select the **Add a group** button.
4. Use the following to create the new **mail-enabled** security group and select the **Add** button.
   - **Type**: Mail-enabled security
    ![M365-ADM-Portal-Mail-Enabled-Sec](images/data-connect-m365-mail-sec.png)
   - **Name**: Consent Request Approvers
    ![M365-ADM-Portal-Mail-Consent-Approvers](images/data-connect-m365-cons-apprv.png)
   - **Email Prefix**: consentrequestapprovers
    ![M365-ADM-Portal-Email-Prefix](images/data-connect-m365-cons-apprv-pref.png)
5. **It can take up to an hour** before the newly created group shows up in the list. Once the group has been created, select it.
    > [!IMPORTANT]
    > Change the View dropdown to **mail-enabled security** if you do not see Consent Request Approvers in the list of groups
6. On the **Members** section of the group dialog, select **Edit**.
7. Add the two users that you enabled the **Global Administrator** role to this new group.

## Enable Microsoft Graph Data Connect in your O365 tenant

In this step you will enable the Microsoft Graph Data Connect service on your Office 365 tenant.

1. While you are still logged into the Microsoft 365 Admin Portal, select the **Settings > Org settings** menu item.
2. Select the **Microsoft Graph Data Connect** service.
![M365-ADM-Portal-MGDC-Toggle](images/data-connect-m365-mgdc-toggle.png)
3. Enable the toggle button at the top of the dialog to **turn Microsoft Graph Data Connect on or off for your entire organization**.
4. Enter **Consent Request Approvers** (or the name of the group you created previously) in the **group of users to make approval decisions** and select **Save**.
