---
title: "List accessPackageLicenseResources"
description: "Get a list of the accessPackageLicenseResource objects and their properties."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: apiPageType
---

# List accessPackageLicenseResources
Namespace: microsoft.graph



Get a list of the [accessPackageLicenseResource](../resources/accesspackagelicenseresource.md) objects and their properties.

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
GET ** Collection URI for microsoft.graph.accessPackageLicenseResource not found
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

If successful, this method returns a `200 OK` response code and a collection of [accessPackageLicenseResource](../resources/accesspackagelicenseresource.md) objects in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "list_accesspackagelicenseresource"
}
-->
``` http
GET https://graph.microsoft.com/v1.0** Collection URI for microsoft.graph.accessPackageLicenseResource not found
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageLicenseResource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageLicenseResource",
      "id": "ef20033d-3243-9d20-2b1d-d163f91c5363",
      "displayName": "String",
      "description": "String",
      "createdDateTime": "String (timestamp)",
      "modifiedDateTime": "String (timestamp)",
      "attributes": [
        {
          "@odata.type": "microsoft.graph.accessPackageResourceAttribute"
        }
      ],
      "skuId": "String"
    }
  ]
}
```

