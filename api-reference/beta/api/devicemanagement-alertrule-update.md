---
title: "Update alertRule"
description: "Update the properties of an alertRule object."
author: "zhishending"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: apiPageType
---

# Update alertRule
Namespace: microsoft.graph.deviceManagement

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [alertRule](../resources/devicemanagement-alertrule.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|CloudPC.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|CloudPC.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/monitoring/alertRules/{alertRuleId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Property|Type|Description|
|:---|:---|:---|
|severity|ruleSeverityType|The severity of the rule. The possible values are: `unknown`, `informational`, `warning`, `critical`, `unknownFutureValue`. Optional.|
|enabled|Boolean|The status of the rule indicating whether the rule is enabled or disabled. When TRUE, indicates the rule is enabled. When FALSE, indicates the rule is disabled. Optional.|
|threshold|[microsoft.graph.deviceManagement.ruleThreshold](../resources/devicemanagement-rulethreshold.md)|The threshold of the rule. Optional.|
|notificationChannels|[microsoft.graph.deviceManagement.notificationChannel](../resources/devicemanagement-notificationchannel.md) collection|he notification channels of the rule selected by user. Optional.|


## Response

If successful, this method returns a `200 OK` response code and an updated [alertRule](../resources/devicemanagement-alertrule.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_alertrule"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/monitoring/alertRules/{alertRuleId}
Content-Type: application/json
Content-length: 457

{
  "@odata.type": "#microsoft.graph.deviceManagement.alertRule",
  "severity": "String",
  "enabled": "Boolean",
  "isSystemRule": "Boolean",
  "threshold": {
    "@odata.type": "microsoft.graph.deviceManagement.ruleThreshold"
  },
  "notificationChannels": [
    {
      "@odata.type": "microsoft.graph.deviceManagement.notificationChannel"
    }
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

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
```
