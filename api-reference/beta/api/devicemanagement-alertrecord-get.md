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
|Delegated (work or school account)|CloudPC.Read.All, CloudPC.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|CloudPC.Read.All, CloudPC.ReadWrite.All|

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#deviceManagement/monitoring/alertRecords/$entity",
  "id": "6c46a7ba-e78a-45e5-a81c-179ab8fd3e8e",
  "displayName": "Upload failure for Device Images",
  "status": "active",
  "severity": "warning",
  "alertRuleId": "30070507-6514-443b-8fa5-06979cedacdf",
  "alertRuleTemplate": "cloudPcImageUploadScenario",
  "detectedDateTime": "2022-03-30T11:55:00.1147865Z",
  "resolvedDateTime": null,
  "lastUpdatedDateTime": "2022-03-31T01:10:20.9648579Z",
  "alertImpact": {
      "value": 2,
      "aggregationType": "count"
  }
}
```