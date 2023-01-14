---
title: "synchronizationInfo resource type"
description: "Contains information about how the object was synchronized. This information is only populated for objects that are synchronized using Azure AD cross-tenant synchronization."
author: "rolyon"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: resourcePageType
---

# synchronizationInfo resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains information about how the object was synchronized. This information is only populated for objects that are synchronized using Azure AD cross-tenant synchronization.


## Properties
|Property|Type|Description|
|:---|:---|:---|
|creationType|synchronizationInfoCreationType| Indicates how the object was synchronized. The possible values are: `tenantToTenantSync`, `unknownFutureValue`. `tenantToTenantSync` indicates that the object was created using Azure AD cross-tenant synchronization.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationInfo",
  "creationType": "String"
}
```

