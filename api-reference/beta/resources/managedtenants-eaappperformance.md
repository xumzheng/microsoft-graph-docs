---
title: "eaAppPerformance resource type"
description: "**TODO: Add Description**"
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# eaAppPerformance resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List eaAppPerformances](../api/managedtenants-managedtenant-list-eaappperformances.md)|[microsoft.graph.managedTenants.eaAppPerformance](../resources/managedtenants-eaappperformance.md) collection|Get a list of the [eaAppPerformance](../resources/managedtenants-eaappperformance.md) objects and their properties.|
|[Create eaAppPerformance](../api/managedtenants-managedtenant-post-eaappperformances.md)|[microsoft.graph.managedTenants.eaAppPerformance](../resources/managedtenants-eaappperformance.md)|Create a new [eaAppPerformance](../resources/managedtenants-eaappperformance.md) object.|
|[Get eaAppPerformance](../api/managedtenants-eaappperformance-get.md)|[microsoft.graph.managedTenants.eaAppPerformance](../resources/managedtenants-eaappperformance.md)|Read the properties and relationships of an [eaAppPerformance](../resources/managedtenants-eaappperformance.md) object.|
|[Update eaAppPerformance](../api/managedtenants-eaappperformance-update.md)|[microsoft.graph.managedTenants.eaAppPerformance](../resources/managedtenants-eaappperformance.md)|Update the properties of an [eaAppPerformance](../resources/managedtenants-eaappperformance.md) object.|
|[Delete eaAppPerformance](../api/managedtenants-managedtenant-delete-eaappperformances.md)|None|Delete an [eaAppPerformance](../resources/managedtenants-eaappperformance.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appFriendlyName|String|**TODO: Add Description**|
|appName|String|**TODO: Add Description**|
|appPublisher|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description**|
|meanTimeToFailureInMinutes|Int32|**TODO: Add Description**|
|tenantDisplayName|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|totalActiveDeviceCount|Int32|**TODO: Add Description**|
|totalAppCrashCount|Int32|**TODO: Add Description**|
|totalAppFreezeCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.eaAppPerformance",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.eaAppPerformance",
  "id": "String (identifier)",
  "appName": "String",
  "appFriendlyName": "String",
  "appPublisher": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "totalActiveDeviceCount": "Integer",
  "totalAppCrashCount": "Integer",
  "totalAppFreezeCount": "Integer",
  "meanTimeToFailureInMinutes": "Integer",
  "lastUpdatedDateTime": "String (timestamp)"
}
```

