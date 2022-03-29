---
title: "monitoring resource type"
description: "The entry point entity type to access all alert related entities and APIs."
author: "zhishending"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: resourcePageType
---

# monitoring resource type

Namespace: microsoft.graph.deviceManagement

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The entry point entity type to access all alert related entities and APIs.

Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get monitoring](../api/devicemanagement-monitoring-get.md)|[microsoft.graph.deviceManagement.monitoring](../resources/devicemanagement-monitoring.md)|Read the properties and relationships of a [monitoring](../resources/devicemanagement-monitoring.md) object.|
|[Update monitoring](../api/devicemanagement-monitoring-update.md)|[microsoft.graph.deviceManagement.monitoring](../resources/devicemanagement-monitoring.md)|Update the properties of a [monitoring](../resources/devicemanagement-monitoring.md) object.|
|[getEffectivePermissions](../api/devicemanagement-monitoring-geteffectivepermissions.md)|String collection|View the effective permissions of the currently authenticated user.|
|[List alertRecords](../api/devicemanagement-monitoring-list-alertrecords.md)|[microsoft.graph.deviceManagement.alertRecord](../resources/devicemanagement-alertrecord.md) collection|Get the alertRecord resources from the alertRecords navigation property.|
|[Create alertRecord](../api/devicemanagement-monitoring-post-alertrecords.md)|[microsoft.graph.deviceManagement.alertRecord](../resources/devicemanagement-alertrecord.md)|Create a new alertRecord object.|
|[List alertRules](../api/devicemanagement-monitoring-list-alertrules.md)|[microsoft.graph.deviceManagement.alertRule](../resources/devicemanagement-alertrule.md) collection|Get the alertRule resources from the alertRules navigation property.|
|[Create alertRule](../api/devicemanagement-monitoring-post-alertrules.md)|[microsoft.graph.deviceManagement.alertRule](../resources/devicemanagement-alertrule.md)|Create a new alertRule object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|The alert id Inherited from [entity](../resources/entity.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|alertRecords|[microsoft.graph.deviceManagement.alertRecord](../resources/devicemanagement-alertrecord.md) collection|The collection of alert rules.|
|alertRules|[microsoft.graph.deviceManagement.alertRule](../resources/devicemanagement-alertrule.md) collection|The collection of records of alert events.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement.monitoring",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement.monitoring",
  "id": "String (identifier)"
}
```
