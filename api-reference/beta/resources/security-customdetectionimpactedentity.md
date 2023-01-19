---
title: "customDetectionImpactedEntity resource type"
description: "Each custom detection rule contains a list of entities which were impacted based on the alert triggered by the custom detection rule."
author: "mmekler"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: resourcePageType
---

# customDetectionImpactedEntity resource type

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

An entity to which the action set in a custom detection rule is applied to.

## Properties
| Property         | Type         | Description                                                                                                                                  |
|:-----------------|:-------------|:---------------------------------------------------------------------------------------------------------------------------------------------|
| entityIdentifier | String       | Unique identifier for the impacted entity.                                                                                                   |
| entityType       | evidenceType | Type of object, such as a file, a process, a device, or a user .The possible values are: `user`, `machine`, `mailbox`, `unknownFutureValue`. |

### evidenceType values

| Value                | Description                                    |
|----------------------|------------------------------------------------|
| `user`               | Impacted entity is a user account              |
| `machine`            | Impacted entity is a device                    |
| `mailbox`            | Impacted entity is a mailbox                   |
| `unknownFutureValue` | unknownFutureValue for evolvable enums pattern |

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.customDetectionImpactedEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.customDetectionImpactedEntity",
  "entityIdentifier": "String",
  "entityType": "String"
}
```

