---
title: "customDetectionActionAdditionalFields resource type"
description: "Additional information about a custom detection rule action"
author: "mmekler"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: resourcePageType
---

# customDetectionActionAdditionalFields resource type

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Additional information about a custom detection rule action.

## Properties
| Property        | Type              | Description                                                                                                                                                                                                                         |
|:----------------|:------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| emailActionType | emailActionType   | Action taken on the email as set in the custom detection rule. The possible values are: `moveToJunk`, `moveToInbox`, `deleteAttachment`, `submitForDetonation`, `delete`, `softDelete`, `moveToDeletedItems`, `unknownFutureValue`. |
| isolationType   | isolationType     | For the isolated device, the type of isolation applied. The possible values are: `full`, `selective`, `unknownFutureValue`.                                                                                                         |
| rbacGroupNames  | String collection | Device groups to which the actions set in the custom detection rule are applied.                                                                                                                                                    |

### emailActionType values

| Member                | Description                                                                                                                                                              |
|-----------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `moveToJunk`          | Moves the email message to the Junk folder                                                                                                                               |
| `moveToInbox`         | Moves the email message to Inbox                                                                                                                                         |
| `deleteAttachment`    | Deletes the email attachment                                                                                                                                             |
| `submitForDetonation` | Submits the email message to check for maliciousness                                                                                                                     |
| `delete`              | Deletes the email message permanently                                                                                                                                    |
| `softDelete`          | Moves the email message to a deleted folder in the cloud. Can be done by admins. End users have to go to the Deleted folder  within the Deleted items folder to do this. |
| `moveToDeletedItems`  | Moves the email message to the end user's Deleted items folder                                                                                                           |
| `unknownFutureValue`  | unknownFutureValue for evolvable enums pattern                                                                                                                           |

### isolationType values

| Member               | Description                                           |
|----------------------|-------------------------------------------------------|
| `full`               | Applies full network isolation to the affected device |
| `selective`          | Applies selective isolation to the affected device    |
| `unknownFutureValue` | unknownFutureValue for evolvable enums pattern        |

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.customDetectionActionAdditionalFields"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.customDetectionActionAdditionalFields",
  "rbacGroupNames": [
    "String"
  ],
  "isolationType": "String",
  "emailActionType": "String"
}
```

