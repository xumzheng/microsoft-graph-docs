---
title: "printRelease complex type"
description: "Represents the job release options supported by a printer."
author: "venkatnagula"
ms.localizationpriority: medium
ms.prod: "cloud-printing"
doc_type: resourcePageType
---

# printRelease complex type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents the job release options supported by a printer.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|releaseType|[printReleaseType](enums.md#printreleasetype-values)|Supported print release type|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printRelease"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printRelease",
  "releaseType": {"@odata.type": "microsoft.graph.printReleaseType"}
}
```
