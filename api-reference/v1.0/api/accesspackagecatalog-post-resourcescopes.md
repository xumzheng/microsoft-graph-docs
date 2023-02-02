---
title: "Create accessPackageResourceScope"
description: "Create a new accessPackageResourceScope object."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: apiPageType
---

# Create accessPackageResourceScope
Namespace: microsoft.graph



Create a new accessPackageResourceScope object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
|:---------------------------------------|:--------------------------------------------|
| Delegated (work or school account)     | EntitlementManagement.ReadWrite.All |
| Delegated (personal Microsoft account) | Not supported. |
| Application                            | EntitlementManagement.ReadWrite.All |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}/resourceScopes
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.

You can specify the following properties when creating an **accessPackageResourceScope**.

**TODO: Remove properties that don't apply**
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description** Optional.|
|description|String|**TODO: Add Description** Optional.|
|isRootScope|Boolean|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and an [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcescope_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}/resourceScopes
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessPackageResourceScope",
  "displayName": "String",
  "description": "String",
  "isRootScope": "Boolean"
}
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceScope"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessPackageResourceScope",
  "id": "a71eef27-7950-97d2-b4fe-7062799af470",
  "displayName": "String",
  "description": "String",
  "isRootScope": "Boolean"
}
```

