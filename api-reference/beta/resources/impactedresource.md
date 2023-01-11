---
title: "impactedResource resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: resourcePageType
---

# impactedResource resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List impactedResources](../api/recommendationbase-list-impactedresources.md)|[impactedResource](../resources/impactedresource.md) collection|Get a list of the [impactedResource](../resources/impactedresource.md) objects and their properties.|
|[Create impactedResource](../api/recommendationbase-post-impactedresources.md)|[impactedResource](../resources/impactedresource.md)|Create a new [impactedResource](../resources/impactedresource.md) object.|
|[Get impactedResource](../api/impactedresource-get.md)|[impactedResource](../resources/impactedresource.md)|Read the properties and relationships of an [impactedResource](../resources/impactedresource.md) object.|
|[Update impactedResource](../api/impactedresource-update.md)|[impactedResource](../resources/impactedresource.md)|Update the properties of an [impactedResource](../resources/impactedresource.md) object.|
|[Delete impactedResource](../api/recommendationbase-delete-impactedresources.md)|None|Delete an [impactedResource](../resources/impactedresource.md) object.|
|[postpone](../api/impactedresource-postpone.md)|[impactedResource](../resources/impactedresource.md)|**TODO: Add Description**|
|[dismiss](../api/impactedresource-dismiss.md)|[impactedResource](../resources/impactedresource.md)|**TODO: Add Description**|
|[complete](../api/impactedresource-complete.md)|[impactedResource](../resources/impactedresource.md)|**TODO: Add Description**|
|[reactivate](../api/impactedresource-reactivate.md)|[impactedResource](../resources/impactedresource.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|addedDateTime|DateTimeOffset|**TODO: Add Description**|
|additionalDetails|[keyValue](../resources/keyvalue.md) collection|**TODO: Add Description**|
|apiUrl|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|lastModifiedBy|String|**TODO: Add Description**|
|lastModifiedDateTime|String|**TODO: Add Description**|
|owner|String|**TODO: Add Description**|
|portalUrl|String|**TODO: Add Description**|
|postponeUntilDateTime|DateTimeOffset|**TODO: Add Description**|
|rank|Int32|**TODO: Add Description**|
|recommendationId|String|**TODO: Add Description**|
|resourceType|String|**TODO: Add Description**|
|status|recommendationStatus|**TODO: Add Description**.The possible values are: `active`, `completedBySystem`, `completedByUser`, `dismissed`, `postponed`, `unknownFutureValue`.|
|subjectId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.impactedResource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.impactedResource",
  "id": "String (identifier)",
  "subjectId": "String",
  "recommendationId": "String",
  "addedDateTime": "String (timestamp)",
  "portalUrl": "String",
  "apiUrl": "String",
  "displayName": "String",
  "resourceType": "String",
  "owner": "String",
  "rank": "Integer",
  "status": "String",
  "additionalDetails": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ],
  "lastModifiedBy": "String",
  "lastModifiedDateTime": "String",
  "postponeUntilDateTime": "String (timestamp)"
}
```

