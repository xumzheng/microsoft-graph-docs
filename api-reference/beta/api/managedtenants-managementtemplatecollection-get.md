---
title: "Get managementTemplateCollection"
description: "Read the properties and relationships of a managementTemplateCollection object."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: apiPageType
---

# Get managementTemplateCollection
Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|ManagedTenants.Read.All, ManagedTenants.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|Not supported.|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementTemplateCollections/{managementTemplateCollectionId}
GET /tenantRelationships/managedTenants/managementTemplates/{managementTemplateId}/managementTemplateCollections/{managementTemplateCollectionId}
```

## Optional query parameters

This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply` and `$select`.

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [managementTemplateCollection](../resources/managedtenants-managementtemplatecollection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_managementtemplatecollection"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementTemplateCollections/{managementTemplateCollectionId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementTemplateCollection"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.managedTenants.managementTemplateCollection",
    "id": "c3a3e023-ef41-5ebb-ba76-b2f53923bed6",
    "displayName": "String",
    "description": "String"
  }
}
```
