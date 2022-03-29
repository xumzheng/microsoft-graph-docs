---
title: "Get alertRecord"
description: "Read the properties and relationships of an alertRecord object."
author: "zhishending"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: apiPageType
---

# Get alertRecord
Namespace: microsoft.graph.deviceManagement

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [alertRecord](../resources/devicemanagement-alertrecord.md) object.

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
GET /deviceManagement/monitoring/alertRecords/{alertRecordId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [alertRecord](../resources/devicemanagement-alertrecord.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_alertrecord"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/monitoring/alertRecords/{alertRecordId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagement.alertRecord"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement.alertRecord",
    "id": "a524f545-5726-239a-4a4d-f153503c960d",
    "displayName": "String",
    "alertImpact": {
      "@odata.type": "microsoft.graph.deviceManagement.alertImpact"
    },
    "status": "String",
    "severity": "String",
    "alertRuleId": "String",
    "alertRuleTemplate": "String",
    "detectedDateTime": "String (timestamp)",
    "resolvedDateTime": "String (timestamp)",
    "lastUpdatedDateTime": "String (timestamp)"
  }
}
```

