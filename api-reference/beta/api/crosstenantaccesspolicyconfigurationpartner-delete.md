---
title: "Delete crossTenantAccessPolicyConfigurationPartner"
description: "Delete a partner-specific configuration in a cross-tenant access policy."
author: "jkdouglas"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Delete crossTenantAccessPolicyConfigurationPartner

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Delete a [partner-specific configuration](../resources/crosstenantaccesspolicyconfigurationpartner.md) in a cross-tenant access policy.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|Policy.ReadWrite.CrossTenantAccess|
|Delegated (personal Microsoft account)|Not applicable|
|Application|Policy.ReadWrite.CrossTenantAccess|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/crossTenantAccessPolicy/partners/{id}
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

### Example 1: Delete a partner-specific configuration

Note: If a configuration includes a user synchronization object, you must first delete the user synchronization object before you can delete the root endpoint /policies/crossTenantAccessPolicy/partners/{id}.

#### Request

<!-- {
  "blockType": "request",
  "name": "delete_crosstenantaccesspolicyconfigurationpartner"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/policies/crossTenantAccessPolicy/partners/9c5d131d-b1c3-4fc4-9e3f-c6557947d551
```

#### Response

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```

### Example 2: Delete the user synchronization for a partner-specific configuration

If you delete the user synchronization object associated with a partner-specific configuration, user synchronization from the source tenant to the target tenant will stop. Also, user objects that already been synchronized will not be cleaned up.

#### Request

<!-- {
  "blockType": "request",
  "name": "delete_crosstenantaccesspolicyconfigurationpartner_identitysynchronization"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/policies/crossTenantAccessPolicy/partners/9c5d131d-b1c3-4fc4-9e3f-c6557947d551/identitySynchronization
```

#### Response

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
