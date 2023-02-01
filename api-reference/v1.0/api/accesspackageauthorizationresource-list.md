---
title: "List accessPackageAuthorizationResources"
description: "Get a list of the accessPackageAuthorizationResource objects and their properties."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: apiPageType
---

# List accessPackageAuthorizationResources
Namespace: microsoft.graph



Get a list of the [accessPackageAuthorizationResource](../resources/accesspackageauthorizationresource.md) objects and their properties.

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
GET ** Collection URI for microsoft.graph.accessPackageAuthorizationResource not found
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

If successful, this method returns a `200 OK` response code and a collection of [accessPackageAuthorizationResource](../resources/accesspackageauthorizationresource.md) objects in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "list_accesspackageauthorizationresource"
}
-->
``` http
GET https://graph.microsoft.com/v1.0** Collection URI for microsoft.graph.accessPackageAuthorizationResource not found
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageAuthorizationResource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageAuthorizationResource",
      "id": "97ead386-f712-8223-2f91-c65bafda0241",
      "displayName": "String",
      "description": "String",
      "createdDateTime": "String (timestamp)",
      "modifiedDateTime": "String (timestamp)",
      "attributes": [
        {
          "@odata.type": "microsoft.graph.accessPackageResourceAttribute"
        }
      ],
      "appId": "String"
    }
  ]
}
```

