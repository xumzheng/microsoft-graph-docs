---
title: "Get accessPackageSharePointGeoLocation"
description: "Read the properties and relationships of an accessPackageSharePointGeoLocation object."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: apiPageType
---

# Get accessPackageSharePointGeoLocation
Namespace: microsoft.graph



Read the properties and relationships of an [accessPackageSharePointGeoLocation](../resources/accesspackagesharepointgeolocation.md) object.

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
GET ** Entity URI for microsoft.graph.accessPackageSharePointGeoLocation not found
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

If successful, this method returns a `200 OK` response code and an [accessPackageSharePointGeoLocation](../resources/accesspackagesharepointgeolocation.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackagesharepointgeolocation"
}
-->
``` http
GET https://graph.microsoft.com/v1.0** Entity URI for microsoft.graph.accessPackageSharePointGeoLocation not found
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageSharePointGeoLocation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessPackageSharePointGeoLocation",
    "id": "a2924703-6c31-fd7e-166d-42d4745897cb",
    "displayName": "String",
    "description": "String",
    "isDefaultEnvironment": "Boolean",
    "createdDateTime": "String (timestamp)",
    "modifiedDateTime": "String (timestamp)",
    "adminUrl": "String"
  }
}
```

