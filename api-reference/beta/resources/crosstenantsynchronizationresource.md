---
title: "crossTenantSynchronizationResource resource type"
description: "Contains origin and synchronization information about a synchronized object from a source Azure AD tenant the object."
author: "rolyon"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# crossTenantSynchronizationResource resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains origin and synchronization information about a synchronized object from a source Azure AD tenant the object. This information is only populated for objects that are synchronized using [Azure AD cross-tenant synchronization](/azure/active-directory/multi-tenant-organizations/cross-tenant-synchronization-overview).

Inherits from [crossTenantResource](../resources/crosstenantresource.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|originTenantId|String|ID of the source Azure AD tenant. Inherited from [crossTenantResource](../resources/crosstenantresource.md).|
|synchronizationInfo|[synchronizationInfo](../resources/synchronizationinfo.md)|Contains information about how the object was synchronized.|

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
  "originTenantId": "String",
  "synchronizationInfo": {
    "@odata.type": "microsoft.graph.synchronizationInfo"
  }
}
```

