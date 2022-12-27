---
title: "crossTenantSynchronizationResource resource type"
description: "**TODO: Add Description**"
author: "rolyon"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# crossTenantSynchronizationResource resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [crossTenantResource](../resources/crosstenantresource.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|originId|String|**TODO: Add Description** Inherited from [crossTenantResource](../resources/crosstenantresource.md).|
|originTenantId|String|**TODO: Add Description** Inherited from [crossTenantResource](../resources/crosstenantresource.md).|
|synchronizationInfo|[synchronizationInfo](../resources/synchronizationinfo.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.crossTenantSynchronizationResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.crossTenantSynchronizationResource",
  "originId": "String",
  "originTenantId": "String",
  "synchronizationInfo": {
    "@odata.type": "microsoft.graph.synchronizationInfo"
  }
}
```

