---
title: "trainingSetting resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: resourcePageType
---

# trainingSetting resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|dueDateTime|DateTimeOffset|**TODO: Add Description**|
|dueDays|Int32|**TODO: Add Description**|
|settingType|trainingSettingType|**TODO: Add Description**.The possible values are: `none`, `microsoft`, `noTraining`, `custom`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|training|[training](../resources/training.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.trainingSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.trainingSetting",
  "dueDays": "Integer",
  "dueDateTime": "String (timestamp)",
  "settingType": "String"
}
```

