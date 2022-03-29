---
title: "alertImpact resource type"
description: "Represents the impact of the alert event. Consists of a number value and the aggregation type."
author: "zhishending"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: resourcePageType
---

# alertImpact resource type

Namespace: microsoft.graph.deviceManagement

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents the impact of the alert event. Consists of a number value and the aggregation type.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aggregationType|[aggregationType](#aggregationtype-values)|The aggregation type of the impact. The possible values are: `count`, `percentage`, `affectedCloudPcCount`, `affectedCloudPcPercentage`, `unknownFutureValue`.|
|value|Int32|The number value of the impact.|

### aggregationType values 

|Member|Description|
|:---|:---|
|count|Indicates the data is aggregated by performing a count on the number of items matching the alert rule conditions.|
|percentage|Indicates the data is shown as a percentage of items matching the alert rule conditions.|
|affectedCloudPcCount|Indicates the total number of Cloud PC's that meet the alert rule conditions.|
|affectedCloudPcPercentage|Indicates the percentage of Cloud PC's that meet the alert rule conditions.|
|unknownFutureValue|Unknown future status (reserved, not used right now).|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagement.alertImpact"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement.alertImpact",
  "value": "Integer",
  "aggregationType": "String"
}
```
