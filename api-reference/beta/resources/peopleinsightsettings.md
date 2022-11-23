---
title: "peopleInsightSettings resource type"
description: "A resource representing a users people insights preferences"
ms.localizationpriority: medium
author: "arunjose"
ms.prod: "users"
doc_type: resourcePageType
---

# peopleInsightSettings resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

User level opt out feature for the people insights feature.

## Methods

| Method                                                 | Return Type                                                   | Description                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [Get](../api/peopleinsightsettings-get.md)       | [peopleInsightSettings](peopleinsightsettings.md) | Read properties of a **peopleInsightSettings** object.                                       |
| [Update](../api/peopleinsightsettings-update.md) | [peopleInsightSettings](peopleinsightsettings.md) | Update all or a subset of the properties of the **peopleInsightSettings** object for a user. |

## Properties
| Property                   | Type                                                  | Description                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| isEnabled     | boolean                         | The user's preference to enable or disable people insights. |

## JSON representation

The following is a JSON definition of the resource.

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.peopleInsightSettings"
} -->

```json
{
    "isEnabled": {"@odata.type":"Edm.boolean"}
}
```
<!-- {
  "type": "#page.annotation",
  "description": "peopleInsightSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


