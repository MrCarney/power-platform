---
title: "Delete users | MicrosoftDocs"
description: Information about deleting users
author: jimholtz
ms.author: jimholtz
ms.reviewer: jimholtz
ms.custom: "admin-security"
ms.service: power-platform
ms.component: pa-admin
ms.topic: conceptual
ms.date: 02/22/2021
search.audienceType: 
  - admin
search.app:
  - D365CE
  - PowerApps
  - Powerplatform
  - Flow
---
# Delete users

Users are deleted in the Microsoft 365 admin center as follows:

1. In the [Microsoft 365 admin center](https://admin.microsoft.com/), go to the **Users** > [Active users](https://go.microsoft.com/fwlink/p/?linkid=834822) page.

2. Select the names of the users that you want to delete, select **More options** (...), and then select **Delete user**.

Although you deleted the user's account, you're still paying for the license. See the next procedure to stop paying for the license. Or, you can assign the license to another user. It won't be assigned to someone automatically. For more information, see [Delete a user from your organization](https://docs.microsoft.com/microsoft-365/admin/add-users/delete-a-user?view=o365-worldwide).

## About deleted users

When a user is deleted from the Microsoft 365 admin center, the user is not removed from environments in which they are active. Instead, the user's status is set to disabled in Dynamics 365.

The following lists the scenarios when a user is deleted:

- If the user is in the environment and has a status of **enabled**, the status will be updated to **disabled**.
- If the user is in the environment and has a status of **disabled**, the status remains as **disabled**.
- If the user is not present in the environment, there is no action taken.

It can take between 30 minutes to 6 hours for a user’s status to be updated in an environment when the user is deleted from the Microsoft 365 admin center.  If you need to update the user status immediately, you can follow the steps in [User diagnostics](troubleshooting-user-needs-read-write-access-organization.md#user-diagnostics) to see what needs to be done to restore the user.

> [!div class="mx-imgBorder"] 
> ![Run diagnostics results](media/run-diagnostics.png "Run diagnostics results")

> [!NOTE]
> A user deleted from the Microsoft 365 admin center is put on the **Deleted user** list for 30 days and can be restored as directed in [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user?view=o365-worldwide).

## About disabled users

When you view the **Users** page in the Power Platform admin center, you can see a list of enabled and disabled users. To view a list of disabled users, follow these steps:

1. In the Power Platform admin center, select an environment.

2. Select **Settings** > **Users + permissions** > **Users**.

3. In the top menu bar, select **Manage users in Dynamics 365**. 

4. From the drop-down menu, choose **Disabled users**. 

## Restore deleted users

To restore a deleted user, follow these steps:

1. In the [Microsoft 365 admin center](https://admin.microsoft.com/), go to the **Users** > [Deleted users](https://go.microsoft.com/fwlink/p/?linkid=834822) page.

2. Select the names of the user that you want to re-enable, select **Restore user**, and then proceed through various pages.

3. Re-assign licenses as needed to the user in the Microsoft 365 admin center.

> [!NOTE]
> You can restore deleted users up to 30 days after deletion.

### See also
[Delete a user from your organization](https://docs.microsoft.com/microsoft-365/admin/add-users/delete-a-user?view=o365-worldwide) <br />
[Troubleshooting: Common user access issues](troubleshooting-user-needs-read-write-access-organization.md)






