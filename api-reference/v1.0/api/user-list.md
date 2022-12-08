---
title: "List users"
description: "Retrieve a list of user objects."
author: "yyuank"
ms.localizationpriority: high
ms.prod: "users"
doc_type: apiPageType
---

# List users

## Permissions

#### Option 1: CURRENT PATTERN

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |



---

#### Option 2: 

Choose the permission marked as least privileged for this API. Only add one of the other permissions if your app requires it. Learn more about [delegated and application permissions](/graph/permissions-overview), and look up a permission in the [permissions reference](/graph/permissions-reference).

| Permission type                         | Least privileged permission  | Other permissions  |
|-----------------------------------------|------------------------------|--------------------|
| Delegated (work or school account)      | User.ReadBasic.All           | User.Read.All      |
| Delegated (personal Microsoft account)  | Not supported.               | Not supported.     |
| Application                             | User.Read.All                | User.ReadWrite.All |

---

#### Option 3:

Choose the permission marked as least privileged for this API. Only add one of the other permissions if your app requires it. To learn more about these permissions, see the [Permissions reference](/graph/permissions-reference).

| Permission type                                                                                                                                               | Least privileged permission | Other permissions  |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------|---------------------|
| [Delegated (work or school account)](/graph/permissions-overview "Delegated permissions allow the application to access data on behalf of a signed-in user.") | User.ReadBasic.All          | User.Read.All      |
| [Delegated (personal Microsoft account)](/graph/permissions-overview "Not all delegated permissions are valid for personal Microsoft accounts.")              | Not supported.              | Not supported.     |
| [Application](/graph/permissions-overview "Application permissions allow the app the access data without signed-in user present.")                            | User.Read.All               | User.ReadWrite.All |

---

#### Option 4:

Choose the permission marked as least privileged for this API. Only add one of the other permissions if your app requires it. Learn more about [delegated and application permissions](/graph/permissions-overview "Delegated permissions allow the application to access data on behalf of a signed-in user. Application permissions allow the app the access data without signed-in user present."), and look up a permission in the [permissions reference](/graph/permissions-reference).

| Permission type                         | Least privileged permission  | Other permissions  |
|-----------------------------------------|------------------------------|--------------------|
| Delegated (work or school account)      | User.ReadBasic.All           | User.Read.All      |
| Delegated (personal Microsoft account)  | Not supported.               | Not supported.     |
| Application                             | User.Read.All                | User.ReadWrite.All |


<!--
Angela's suggestion: 
•	Choose one of the following permissions that is the least privileged required by your app.
•	A delegated permission limits data access to within the signed-in user's privileges. An application permission provides the exact privileges it implies.
•	Learn more about delegated and application permissions, and look up a permission in the permissions reference.

Comments:
Shorten - one sentence
Later for the RBAC boilerplate, add custom roles.
-->