---
title: "Create alert rule"
description: "Create an alertRule object."
author: "zhishending"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: apiPageType
---

# Add educationClass to educationSchool

Namespace: microsoft.graph.deviceManagement

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create an alertRule object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account)|CloudPC.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|CloudPC.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /deviceManagement/monitoring/alertRules
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
|displayName|String|The display name of the rule.|
|description|String|The rule description.|
|isSystemRule|Boolean|Indicates whether the rule is a system rule. System rules are built-in and only a few properties can be edited. When TRUE, the rule is a system rule. When FALSE, the rule is a custom defined rule and can be edited.|
|alertRuleTemplate|alertRuleTemplate|The rule template of the rule. The possible values are: `cloudPcProvisionScenario`, `cloudPcImageUploadScenario`, `cloudPcOnPremiseNetworkConnectionCheckScenario`, `unknownFutureValue`.|
|severity|ruleSeverityType|The severity of the rule. The possible values are: `unknown`, `informational`, `warning`, `critical`, `unknownFutureValue`.|
|enabled|Boolean|The status of the rule indicating whether the rule is enabled or disabled. When TRUE, indicates the rule is enabled. When FALSE, indicates the rule is disabled.|
|threshold|[microsoft.graph.deviceManagement.ruleThreshold](../resources/devicemanagement-rulethreshold.md)|The threshold of the rule.|
|notificationChannels|[microsoft.graph.deviceManagement.notificationChannel](../resources/devicemanagement-notificationchannel.md) collection|he notification channels of the rule selected by user.|

## Response
If successful, this method returns a `201 Created` response code and an [alertRule](../resources/devicemanagement-alertrule.md) object in the response body.

## Example

##### Request
<!-- {
  "blockType": "request",
  "name": "post_alertrule"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/monitoring/alertRules
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

##### Response 
<!-- {
  "blockType": "response",
}
-->
``` http
HTTP/1.1 201 CREATED
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
