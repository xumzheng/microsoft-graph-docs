---
title: "crossTenantResource resource type"
description: "Contains origin information about a synchronized object from a source Azure AD tenant."
author: "rolyon"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# crossTenantResource resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains origin information about a synchronized object from a source Azure AD tenant. This information is only populated for objects that are synchronized using [Azure AD cross-tenant synchronization](/azure/active-directory/multi-tenant-organizations/cross-tenant-synchronization-overview).

This is an abstract type that's inherited by the [crossTenantSynchronizationResource](crosstenantsynchronizationresource.md) resource type.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|originId|String|ID of the original object in the source Azure AD tenant the object was synchronized from.|
|originTenantId|String|ID of the source Azure AD tenant.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.crossTenantResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.crossTenantResource",
  "originId": "String",
  "originTenantId": "String"
}
```

