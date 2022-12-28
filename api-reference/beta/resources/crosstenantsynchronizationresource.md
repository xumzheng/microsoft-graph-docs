---
title: "crossTenantSynchronizationResource resource type"
description: "Contains object and synchronization information about the original object in the source Azure AD tenant the object was synchronized from."
author: "rolyon"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# crossTenantSynchronizationResource resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains object and synchronization information about the original object in the source Azure AD tenant the object was synchronized from. This information is only populated for objects that are synchronized using Azure AD cross-tenant synchronization.

Inherits from [crossTenantResource](../resources/crosstenantresource.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|originId|String|ID of the original object in the source Azure AD tenant the object was synchronized from. Inherited from [crossTenantResource](../resources/crosstenantresource.md).|
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
  "originId": "String",
  "originTenantId": "String",
  "synchronizationInfo": {
    "@odata.type": "microsoft.graph.synchronizationInfo"
  }
}
```

