---
title: "Govern membership and ownership of Azure AD groups using the privileged identity management (PIM) API"
description: "Privileged Identity Management (PIM) is a feature of Azure AD Identity Governance that enables you to manage, control, and monitor access to important resources in your organization."
author: "rkarim-ms"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
ms.date: 03/13/2023
---

# Govern membership and ownership of Azure AD groups using PIM

With Azure Active Directory (Azure AD), part of Microsoft Entra, you can provide users just-in-time membership in the group and just-in-time ownership of the group using the [Azure AD Privileged Identity Management for Groups](/azure/active-directory/privileged-identity-management/concept-pim-for-groups) feature. These groups can be used to govern access to a variety of scenarios that include Azure AD roles, Azure roles, as well as Azure SQL, Azure Key Vault, Intune, other application roles, and 3rd party applications.

The Microsoft Graph API for PIM for Groups allows you to govern privileged access using PIM for Groups and activate the ownership or membership of an Azure AD security group or Microsoft 365 group. This article introduces the governance capabilities of the APIs for PIM for Groups in Microsoft Graph.

**PIM for Groups API for managing group owner and member assignments**

PIM allows you to manage active assignments for users to groups by creating permanent assignments or temporary assignments. Use the privilegedAccessGroupAssignmentScheduleRequestresource type and its related methods to manage assignments for users to groups.

The following table lists scenarios for using PIM for Groups to manage assignments for users to groups and the corresponding APIs to call.

| **Scenarios** | **API** |
| --- | --- |
| An administrator assigns a principal active membership to a group | Create privilegedAccessGroupAssignmentScheduleRequest |
| An administrator renews, updates, extends, or removes a principal from their active membership in a group | Create privilegedAccessGroupAssignmentScheduleRequest |
| An administrator queries all requests for active membership assignments for a group | List privilegedAccessGroupAssignmentScheduleRequests |
| An administrator lists all requests for active group membership that are past, future, and current assignments | List privilegedAccessGroupAssignmentSchedules |
| An administrator lists all active membership assignments for a group | List privilegedAccessGroupAssignmentScheduleInstances |
| An administrator queries a member assignment for a group and its details | Get privilegedAccessGroupAssignmentScheduleRequest |
| A principal queries their member assignment requests and the details | privilegedAccessGroupAssignmentScheduleRequest: filterByCurrentUser |
| A principal performs just-in-time and time-bound activation of their _eligible_ member assignment for a group | Create privilegedAccessGroupAssignmentScheduleRequest |
| A principal cancels a member assignment request they created | privilegedAccessGroupAssignmentScheduleRequest: cancel |
| A principal that has activated their eligible member assignment deactivates it when they no longer need access | Create privilegedAccessGroupAssignmentScheduleRequest |
| A principal deactivates, extends, or renews their own member assignment. | Create privilegedAccessGroupAssignmentScheduleRequest |

**PIM for Groups API for managing group owner and member eligibilities**

Your principals may not require permanent member assignments because they may not require the privileges granted through the privileged assignment all the time. In this case, PIM also allows you to create member eligibilities and assign them to the principals. With member eligibilities, the principal activates the assignment when they need to perform privileged tasks. The activation is always time-bound for a maximum of 8 hours. The eligibility can also be permanent or temporary. Use the privilegedAccessGroupEligibilityScheduleRequestresource type and its related methods to manage eligibilities for PIM for Groups.

The following table lists scenarios for using PIM to manage eligibilities for PIM for Groups and the corresponding APIs to call.

| **Scenarios** | **API** |
| --- | --- |
| An administrator creates and assigns a member eligibility for a user to a group


An administrator assigns a temporary member eligibility for a user to a group | Create privilegedAccessGroupEligibilityScheduleRequest |
| An administrator renews, updates, extends, or removes role eligibilities | Create privilegedAccessGroupEligibilityScheduleRequest |
| An administrator queries all role eligibilities and their details | List privilegedAccessGroupEligibilityScheduleRequests |
| An administrator queries a role eligibility and its details | Get privilegedAccessGroupEligibilityScheduleRequest |
| An administrator cancels a role eligibility request they created | privilegedAccessGroupEligibilityScheduleRequest:cancel |
| A principal queries their role eligibilities and the details | [privilegedAccessGroupEligibilityScheduleRequest: filterByCurrentUser](/graph/api/unifiedroleeligibilityschedulerequest-filterbycurrentuser) |
| A principal deactivates, extends, or renews their own role eligibility. | Create privilegedAccessGroupEligibilityScheduleRequest |

**PIM for Groups and identity Security with Zero Trust**

PIM APIs support organizations to adopt a Zero Trust approach to secure the identities in their organization. For more information about Zero Trust, see [Securing identity with Zero Trust](/security/zero-trust/deploy/identity#secure-privileged-access-with-privileged-identity-management).

**Permissions and Privileges**

To call the Create privilegedAccessGroupAssignmentScheduleRequest and Create privilegedAccessGroupEligibilityScheduleRequestAPIs with admin actions, the calling app must:

- Have a _Global Administrator_ or _Privileged Role Administrator_ role
- Be granted the following permission:
  - PrivilegedAccess.ReadWrite.AzureADGroup

The app must also be assigned the appropriate permissions to retrieve their role assignments and eligibilities, or call the Create privilegedAccessGroupAssignmentScheduleRequest and Create privilegedAccessGroupEligibilityScheduleRequest APIs with user actions.

For more information about permissions to call PIM APIs, see the [Microsoft Graph permissions reference: Role management permissions](/graph/permissions-reference#role-management-permissions).

**Licensing**

The PIM API requires an Azure AD Premium P2 license. For more information, see [License requirements to use Privileged Identity Management](/azure/active-directory/privileged-identity-management/subscription-requirements).

**See also**

- [What is Azure AD Identity Governance?](/azure/active-directory/governance/identity-governance-overview)
- [What is Azure AD Privileged Identity Management?](/azure/active-directory/privileged-identity-management/pim-configure)
- [Privileged Identity Management (PIM) for Groups (preview)](/azure/active-directory/privileged-identity-management/concept-pim-for-groups)