---
title: "List partners"
description: "Get a list of all partner configurations within a cross-tenant access policy."
author: "jkdouglas"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# List partners

Namespace: microsoft.graph

Get a list of all partner configurations within a cross-tenant access policy. You can also use the `$expand` parameter to list the user synchronization policy for all partner configurations.

## Permissions

Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "crosstenantaccesspolicy_list_partners" } -->
[!INCLUDE [permissions-table](../includes/permissions/crosstenantaccesspolicy-list-partners-permissions.md)]

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/crossTenantAccessPolicy/partners
```

## Optional query parameters

This method supports the `$select` and `$expand` OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [crossTenantAccessPolicyConfigurationPartner](../resources/crosstenantaccesspolicyconfigurationpartner.md) objects in the response body.

## Examples

### Example 1: List all partner configurations within a cross-tenant access policy

The following example shows how to list all partner configurations within a cross-tenant access policy.

#### Request

The following is an example of the request.

<!-- {
  "blockType": "request",
  "name": "list_crosstenantaccesspolicyconfigurationpartner"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/policies/crossTenantAccessPolicy/partners
```

#### Response

The following is an example of the response.

>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.crossTenantAccessPolicyConfigurationPartner)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "tenantId": "123f4846-ba00-4fd7-ba43-dac1f8f63013",
      "inboundTrust": null,
      "automaticUserConsentSettings": {
        "inboundAllowed": null,
        "outboundAllowed": null
      },
      "b2bCollaborationInbound": null,
      "b2bCollaborationOutbound": null,
      "b2bDirectConnectOutbound": null,
      "b2bDirectConnectInbound": {
        "usersAndGroups": {
          "accessType": "allowed",
          "targets": [
            {
              "target": "AllUsers",
              "targetType": "user"
            }
          ]
        },
        "applications": {
          "accessType": "allowed",
          "targets": [
            {
              "target": "Office365",
              "targetType": "application"
            }
          ]
        }
      }
    }
  ]
}
```

### Example 2: List the user synchronization policy for all partner configurations

The following example uses the `$expand` parameter to list the user synchronization policy for all partner configurations.

#### Request

The following is an example of the request.

<!-- {
  "blockType": "request",
  "name": "list_crosstenantidentitysyncpolicypartner"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/crossTenantAccessPolicy/partners?$select=tenantId&$expand=identitySynchronization
```

#### Response

The following is an example of the response.

>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.crossTenantIdentitySyncPolicyPartner)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "tenantId": "9c5d131d-b1c3-4fc4-9e3f-c6557947d551",
      "identitySynchronization": {
        "tenantId": "9c5d131d-b1c3-4fc4-9e3f-c6557947d551",
        "displayName": "Fabrikam",
        "userSyncInbound": {
          "isSyncAllowed": true
        }
      }
    }
  ]
}
```
