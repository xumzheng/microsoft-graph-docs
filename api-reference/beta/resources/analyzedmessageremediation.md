---
title: "analyzedMessageRemediation resource type"
description: "analyzedMessageRemediation object definition"
author: "smkjain8"
ms.localizationpriority: medium
ms.prod: "analyzedmessage-remediations"
doc_type: resourcePageType
---

# analyzedMessageRemediation resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Create analyzedMessageRemediation](../api/analyzedmessageremediation-post-analyzedmessageremediations.md)|[analyzedMessageRemediation](../resources/analyzedmessageremediation.md)|Create a new [analyzedMessageRemediation](../resources/analyzedmessageremediation.md) object.|


## Properties
|Property|Type|Description|
|:---|:---|:---|
|bulkId|String|The unique id to identify the Admin Action|
|id|String|Inherited from [entity](../resources/entity.md).|


## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.analyzedMessageRemediation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.analyzedMessageRemediation",
  "id": "String (identifier)",
  "bulkId": "String"
}
```

