---
title: "eaDeviceAppPerformance resource type"
description: "**TODO: Add Description**"
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"doc_type: resourcePageType
---

# eaDeviceAppPerformance resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List eaDeviceAppPerformances](../api/managedtenants-managedtenant-list-eadeviceappperformances.md)|[microsoft.graph.managedTenants.eaDeviceAppPerformance](../resources/managedtenants-eadeviceappperformance.md) collection|Get a list of the [eaDeviceAppPerformance](../resources/managedtenants-eadeviceappperformance.md) objects and their properties.|
|[Create eaDeviceAppPerformance](../api/managedtenants-managedtenant-post-eadeviceappperformances.md)|[microsoft.graph.managedTenants.eaDeviceAppPerformance](../resources/managedtenants-eadeviceappperformance.md)|Create a new [eaDeviceAppPerformance](../resources/managedtenants-eadeviceappperformance.md) object.|
|[Get eaDeviceAppPerformance](../api/managedtenants-eadeviceappperformance-get.md)|[microsoft.graph.managedTenants.eaDeviceAppPerformance](../resources/managedtenants-eadeviceappperformance.md)|Read the properties and relationships of an [eaDeviceAppPerformance](../resources/managedtenants-eadeviceappperformance.md) object.|
|[Update eaDeviceAppPerformance](../api/managedtenants-eadeviceappperformance-update.md)|[microsoft.graph.managedTenants.eaDeviceAppPerformance](../resources/managedtenants-eadeviceappperformance.md)|Update the properties of an [eaDeviceAppPerformance](../resources/managedtenants-eadeviceappperformance.md) object.|
|[Delete eaDeviceAppPerformance](../api/managedtenants-managedtenant-delete-eadeviceappperformances.md)|None|Delete an [eaDeviceAppPerformance](../resources/managedtenants-eadeviceappperformance.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appFriendlyName|String|**TODO: Add Description**|
|appName|String|**TODO: Add Description**|
|appPublisher|String|**TODO: Add Description**|
|appVersion|String|**TODO: Add Description**|
|deviceId|String|**TODO: Add Description**|
|deviceManufacturer|String|**TODO: Add Description**|
|deviceModel|String|**TODO: Add Description**|
|deviceName|String|**TODO: Add Description**|
|healthStatus|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|isLatestUsedVersion|Int32|**TODO: Add Description**|
|isMostUsedVersion|Int32|**TODO: Add Description**|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description**|
|tenantDisplayName|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|totalAppCrashCount|Int32|**TODO: Add Description**|
|totalAppFreezeCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.eaDeviceAppPerformance",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.eaDeviceAppPerformance",
  "id": "String (identifier)",
  "appName": "String",
  "appFriendlyName": "String",
  "appPublisher": "String",
  "appVersion": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "healthStatus": "String",
  "totalAppCrashCount": "Integer",
  "totalAppFreezeCount": "Integer",
  "isLatestUsedVersion": "Integer",
  "isMostUsedVersion": "Integer",
  "lastUpdatedDateTime": "String (timestamp)"
}
```

