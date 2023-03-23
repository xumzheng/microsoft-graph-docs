---
title: "Microsoft Graph permissions reference "
description: "Microsoft Graph exposes granular permissions that control the access that apps have to resources, like users, groups, and mail. As a developer, you decide which permissions for Microsoft Graph your app requests."
author: "FaithOmbongi"
ms.author: ombongifaith
ms.reviewer: jackson.woods
ms.localizationpriority: high
ms.topic: reference
ms.prod: "applications"
ms.custom: graphiamtop20, scenarios:getting-started
ms.date: 02/17/2022
---

# Microsoft Graph permissions reference

For an app to access data in Microsoft Graph, the user or administrator must grant it the permissions it needs. This topic lists the delegated and application permissions exposed by Microsoft Graph. For guidance about how to use the permissions, see the [Overview of Microsoft Graph permissions](permissions-overview.md).

<!--To find the unique identifiers for all permissions, see [All permissions and IDs](#all-permissions-and-ids).-->

[!INCLUDE [auth-use-least-privileged](../includes/auth-use-least-privileged.md)]

## All permissions

#### AccessReview.Read.All

|  | Application | Delegated |
|--|--|--|
| Identifier | d07a8cc0-3d51-4b77-b3b0-32704d1f69fa | ebfcd32b-babb-40f4-a14b-42706e83bd28 |
| Display name | Read all access reviews | Read all access reviews that user can access |
| Description | Allows the app to read access reviews, reviewers, decisions and settings in the organization, without a signed-in user. | Allows the app to read access reviews, reviewers, decisions and settings that the signed-in user has access to in the organization. |

#### AgreementAcceptance.Read

|              | Application    | Delegated                                                                                |
|--------------|----------------|------------------------------------------------------------------------------------------|
| Identifier   | Not available. | 0b7643bb-5336-476f-80b5-18fbfbc91806                                                     |
| Display name | Not available. | Read user terms of use acceptance statuses                                               |
| Description  | Not available. | Allows the app to read terms of use acceptance statuses on behalf of the signed-in user. |