---
title: "chatIdentity resource type"
description: "Represents the identity of a chat in Microsoft Teams."
author: "Kanaka"
doc_type: resourcePageType
ms.localizationpriority: medium
ms.prod: "teamwork"
---
# chatIdentity resource type

Contains basic identification information about a chat in Microsoft Teams.

## Properties

| Property   | Type |Description|
|:---------------|:--------|:----------|
|chatId|string|  The identity of the chat in which the message was posted.|
|tenantId|string|  The identity of the tenantId in which the chat belongs to.|

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    
  ],
  "@odata.type": "microsoft.graph.chatIdentity"
}-->

```json
{
   "chatId":"string",
   "tenantId":"string",
}
```

<!-- uuid: 4DFA000D-1A5F-4299-B3DD-835E4DD2F3BF
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat identity  resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
