---
title: "Customizing people insights privacy in Microsoft Graph"
description: "The overview of customizing of people insights at the organization level"
author: "PeterNjorogeMS"
ms.localizationpriority: high
ms.prod: "insights"
ms.custom: scenarios:getting-started
---

# Customizing people insights privacy in Microsoft Graph  (preview)

People insights represent connections of people who are [relevant to or working with](people-example.md#including-a-person-as-relevant-or-working-with) one another within the same organization, based on public relationships between the people. These insights can be displayed in Delve and the profile card, and returned by the [people API](/graph/api/user-list-people?view=graph-rest-beta&preserve-view=true).


## How to customize people insights? 

By default, the display or return of people insights is enabled for an organization. Administrators with the global administrator role can customize this behavior for an organization using REST APIs and the appropriate permissions. They can customize by setting properties of the [insightsSettings](/graph/api/resources/insightssettings?view=graph-rest-beta&preserve-view=true) resource in the following ways:

- Disable people insights for all users in the organization, by setting the **isEnabledInOrganization** property of the **insightsSettings** resource to false. (By default, the **isEnabledInOrganization** property is true.)

- Disable people insights for a subset of users, by assigning these users to an Azure AD group, and setting the **disabledForGroup** property to the ID of that group. Find out more about [creating a group and adding users as members](/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal). 

Use the [update](/graph/api/insightssettings-update?view=graph-rest-beta&preserve-view=true) operation to set the **isEnabledInOrganization** or **disabledForGroup** properties accordingly for people insights. 

Keep the following in mind when updating item insights settings: 
* People insights settings are available only in the beta endpoint. 
* The update operation doesn’t check if a group exists. Make sure to get the correct ID of the Azure AD group from the Azure portal, that the group exists, and that the intended users have been added to the group. If the group doesn’t exist, then no changes will be made for any user in the organization. 
* Updating **insightsSettings** can take up to 8 hours before they take effect. 

## Behavior changes in UI and APIs 

Disabling people insights means that the data will not be generated for the given user; it doesn’t affect search and ranking of results.

This is where the changes will be noticeable, the list will be revised in the future.  
* Microsoft 365 [profile card](https://support.microsoft.com/office/profile-cards-in-microsoft-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501)
* User profile in Delve
