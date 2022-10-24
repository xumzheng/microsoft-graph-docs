---
title: "eaDeviceHealthStatus resource type"
description: "**TODO: Add Description**"
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"doc_type: resourcePageType
---

# eaDeviceHealthStatus resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List eaDeviceHealthStatus](../api/managedtenants-managedtenant-list-eadevicehealthstatuses.md)|[microsoft.graph.managedTenants.eaDeviceHealthStatus](../resources/managedtenants-eadevicehealthstatus.md) collection|Get a list of the [eaDeviceHealthStatus](../resources/managedtenants-eadevicehealthstatus.md) objects and their properties.|
|[Create eaDeviceHealthStatus](../api/managedtenants-managedtenant-post-eadevicehealthstatuses.md)|[microsoft.graph.managedTenants.eaDeviceHealthStatus](../resources/managedtenants-eadevicehealthstatus.md)|Create a new [eaDeviceHealthStatus](../resources/managedtenants-eadevicehealthstatus.md) object.|
|[Get eaDeviceHealthStatus](../api/managedtenants-eadevicehealthstatus-get.md)|[microsoft.graph.managedTenants.eaDeviceHealthStatus](../resources/managedtenants-eadevicehealthstatus.md)|Read the properties and relationships of an [eaDeviceHealthStatus](../resources/managedtenants-eadevicehealthstatus.md) object.|
|[Update eaDeviceHealthStatus](../api/managedtenants-eadevicehealthstatus-update.md)|[microsoft.graph.managedTenants.eaDeviceHealthStatus](../resources/managedtenants-eadevicehealthstatus.md)|Update the properties of an [eaDeviceHealthStatus](../resources/managedtenants-eadevicehealthstatus.md) object.|
|[Delete eaDeviceHealthStatus](../api/managedtenants-managedtenant-delete-eadevicehealthstatuses.md)|None|Delete an [eaDeviceHealthStatus](../resources/managedtenants-eadevicehealthstatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|blueScreenCount|Int32|**TODO: Add Description**|
|bootTotalDurationInSeconds|Double|**TODO: Add Description**|
|deviceId|String|**TODO: Add Description**|
|deviceMake|String|**TODO: Add Description**|
|deviceModel|String|**TODO: Add Description**|
|deviceName|String|**TODO: Add Description**|
|healthStatus|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description**|
|osVersion|String|**TODO: Add Description**|
|primaryDiskType|String|**TODO: Add Description**|
|restartCount|Int32|**TODO: Add Description**|
|startupPerformanceScore|Double|**TODO: Add Description**|
|tenantDisplayName|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|topProcesses|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.eaDeviceHealthStatus",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.eaDeviceHealthStatus",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "deviceModel": "String",
  "deviceMake": "String",
  "osVersion": "String",
  "primaryDiskType": "String",
  "startupPerformanceScore": "Double",
  "bootTotalDurationInSeconds": "Double",
  "restartCount": "Integer",
  "blueScreenCount": "Integer",
  "healthStatus": "String",
  "topProcesses": "String",
  "lastUpdatedDateTime": "String (timestamp)"
}
```

