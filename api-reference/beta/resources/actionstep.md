---
title: "actionStep resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: resourcePageType
---

# actionStep resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionUrl|[actionUrl](../resources/actionurl.md)|**TODO: Add Description**|
|stepNumber|Int64|**TODO: Add Description**|
|text|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.actionStep"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.actionStep",
  "stepNumber": "Integer",
  "text": "String",
  "actionUrl": {
    "@odata.type": "microsoft.graph.actionUrl"
  }
}
```

