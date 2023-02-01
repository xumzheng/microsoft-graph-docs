---
title: "Get accessPackagePowerPlatformEnvironment"
description: "Read the properties and relationships of an accessPackagePowerPlatformEnvironment object."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: apiPageType
---

# Get accessPackagePowerPlatformEnvironment
Namespace: microsoft.graph



Read the properties and relationships of an [accessPackagePowerPlatformEnvironment](../resources/accesspackagepowerplatformenvironment.md) object.

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
GET ** Entity URI for microsoft.graph.accessPackagePowerPlatformEnvironment not found
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

If successful, this method returns a `200 OK` response code and an [accessPackagePowerPlatformEnvironment](../resources/accesspackagepowerplatformenvironment.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackagepowerplatformenvironment"
}
-->
``` http
GET https://graph.microsoft.com/v1.0** Entity URI for microsoft.graph.accessPackagePowerPlatformEnvironment not found
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackagePowerPlatformEnvironment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessPackagePowerPlatformEnvironment",
    "id": "4e020da8-3924-7dec-6ef4-582bef76d8f3",
    "displayName": "String",
    "description": "String",
    "isDefaultEnvironment": "Boolean",
    "createdDateTime": "String (timestamp)",
    "modifiedDateTime": "String (timestamp)",
    "environmentId": "String",
    "applicationUrl": "String"
  }
}
```

