---
title: "Delete crossTenantIdentitySyncPolicyPartner"
description: "Delete the user synchronization policy for a partner-specific configuration."
author: "rolyon"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Delete crossTenantIdentitySyncPolicyPartner

Namespace: microsoft.graph

Delete the user synchronization policy for a partner-specific configuration.

## Permissions

Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "crosstenantidentitysyncpolicypartner_delete" } -->
[!INCLUDE [permissions-table](../includes/permissions/crosstenantidentitysyncpolicypartner-delete-permissions.md)]

The signed-in user must also be assigned the following minimum [directory role](/azure/active-directory/roles/permissions-reference):

* Security Administrator

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /policies/crossTenantAccessPolicy/partners/{id}/identitySynchronization
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request

The following is an example of a request.

<!-- {
  "blockType": "request",
  "name": "delete_crosstenantidentitysyncpolicypartner"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/policies/crossTenantAccessPolicy/partners/9c5d131d-b1c3-4fc4-9e3f-c6557947d551/identitySynchronization
```

### Response

The following is an example of the response.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
