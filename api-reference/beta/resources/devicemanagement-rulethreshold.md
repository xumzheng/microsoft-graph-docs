---
title: "ruleThreshold resource type"
description: "Includes information about an alert rule's threshold settings."
author: "zhishending"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: resourcePageType
---

# ruleThreshold resource type

Namespace: microsoft.graph.deviceManagement

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Includes information about an alert rule's threshold settings.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aggregation|aggregationType|Indicates the built-in aggregation methods. The possible values are: `count`, `percentage`, `affectedCloudPcCount`, `affectedCloudPcPercentage`, `unknownFutureValue`.|
|operator|operatorType|Indicates the built-in operator. The possible values are: `greaterOrEqual`, `equal`, `greater`, `less`, `lessOrEqual`, `notEqual`, `unknownFutureValue`.|
|target|Int32|Target threshold value.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagement.ruleThreshold"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement.ruleThreshold",
  "aggregation": "String",
  "operator": "String",
  "target": "Integer"
}
```
