---
title: "monitoring: getEffectivePermissions"
description: "View the effective permissions of the currently authenticated user."
author: "zhishending"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: apiPageType
---

# monitoring: getEffectivePermissions
Namespace: microsoft.graph.deviceManagement

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

View the effective permissions of the currently authenticated user.


## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|CloudPC.ReadWrite.All|
|Delegated (work or school account)|CloudPC.Read.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|CloudPC.ReadWrite.All|
|Application|CloudPC.Read.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /monitoring/getEffectivePermissions
GET /deviceManagement/monitoring/getEffectivePermissions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a String collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "monitoringthis.geteffectivepermissions"
}
-->
``` http
GET https://graph.microsoft.com/beta/monitoring/getEffectivePermissions
```


### Response
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    "String"
  ]
}
```

