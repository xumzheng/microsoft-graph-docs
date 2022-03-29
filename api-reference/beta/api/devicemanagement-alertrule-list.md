---
title: "List alertRules"
description: "Get a list of the alertRule objects and their properties."
author: "zhishending"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: apiPageType
---

# List alertRules
Namespace: microsoft.graph.deviceManagement

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [alertRule](../resources/devicemanagement-alertrule.md) objects and their properties.

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
GET /deviceManagement/monitoring/alertRules
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [alertRule](../resources/alertrule.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_alertrule"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/monitoring/alertRules
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.deviceManagement.alertRule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagement.alertRule",
      "id": "76c904ea-cb78-d9dd-cfff-0bc4d089ac24",
      "displayName": "String",
      "description": "String",
      "severity": "String",
      "enabled": "Boolean",
      "isSystemRule": "Boolean",
      "alertRuleTemplate": "String",
      "threshold": {
        "@odata.type": "microsoft.graph.deviceManagement.ruleThreshold"
      },
      "notificationChannels": [
        {
          "@odata.type": "microsoft.graph.deviceManagement.notificationChannel"
        }
      ]
    }
  ]
}
```
