---
title: "List accessPackageAuthorizationScopes"
description: "Get a list of the accessPackageAuthorizationScope objects and their properties."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: apiPageType
---

# List accessPackageAuthorizationScopes
Namespace: microsoft.graph



Get a list of the [accessPackageAuthorizationScope](../resources/accesspackageauthorizationscope.md) objects and their properties.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET ** Collection URI for microsoft.graph.accessPackageAuthorizationScope not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [accessPackageAuthorizationScope](../resources/accesspackageauthorizationscope.md) objects in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "list_accesspackageauthorizationscope"
}
-->
``` http
GET https://graph.microsoft.com/v1.0** Collection URI for microsoft.graph.accessPackageAuthorizationScope not found
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAuthorizationScope)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageAuthorizationScope",
      "id": "2be525ee-6609-40be-cf7f-6408d133eab7",
      "displayName": "String",
      "description": "String",
      "isRootScope": "Boolean",
      "scopeId": "String"
    }
  ]
}
```

