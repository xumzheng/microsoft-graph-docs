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

#### Option 1: 

Choose the permission marked as least privileged for this API. Use a higher privileged permission only if your app requires it. For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

| Permission type                        | Least privileged permission | Higher privileged permissions                                                  |
|-----------------------------------------|------------------------------|---------------------------------------------------------------------------------|
| Delegated (work or school account)     | User.ReadBasic.All          | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |
| Delegated (personal Microsoft account) | Not supported.              | Not supported.                                                                 |
| Application                            | User.Read.All               | User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All                |


---------------------------------------------------------

#### Option 2:

Choose the permission marked as least privileged for this API. Use a higher privileged permission only if your app requires it. For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types "Delegated permissions allow the application to access data on behalf of a signed-in user. Application permissions allow the app the access data without signed-in user present."). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

| Permission type                        | Least privileged permission | Higher privileged permissions                                                  |
|-----------------------------------------|------------------------------|---------------------------------------------------------------------------------|
| Delegated (work or school account)     | User.ReadBasic.All          | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |
| Delegated (personal Microsoft account) | Not supported.              | Not supported.                                                                 |
| Application                            | User.Read.All               | User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All                |


---------------------------------------------------------
<!--

Choose the permission marked as least privileged for this API. Use a higher privileged permission only if your app requires it. To learn more about these permissions, see the [Permissions reference](/graph/permissions-reference).

| Permission type                                                                                                                                                                     | Least privileged permission | Higher privileged permissions                                                  |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------|---------------------------------------------------------------------------------|
| [Delegated (work or school account)](/graph/permissions-overview#delegated-permissions "Delegated permissions allow the application to access data on behalf of a signed-in user.") | User.ReadBasic.All          | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |
| [Delegated (personal Microsoft account)](/graph/permissions-overview#delegated-permissions "Not all delegated permissions are valid for personal Microsoft accounts.")              | Not supported.              | Not supported.                                                                 |
| [Application](/graph/permissions-overview#application-permissions "Application permissions allow the app the access data without signed-in user present.")                          | User.Read.All               | User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All                |

-->