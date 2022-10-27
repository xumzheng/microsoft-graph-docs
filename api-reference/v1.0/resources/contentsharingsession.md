---
title: "contentSharingSession resource type"
description: "Represents a content sharing session in a call."
author: "satyakonmsft"
ms.localizationpriority: medium
ms.prod: "cloud-communications"
doc_type: resourcePageType
---

# contentSharingSession resource type

Namespace: microsoft.graph

Represents a content sharing session in a call. When a content sharing session starts in a call, a notification is sent if the isContentSharingNotificationEnabled is set to true in the [incomingCallOptions](incomingcalloptions.md) (when answering a call) or [outgoingCallOptions](outgoingcalloptions.md) (when creating a call or joining a meeting)

## contentSharingSession Notifications

#### Notification - content sharing started

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "created",
      "resourceUrl": "/communications/calls/421f4c00-4436-4c3a-9d9a-c4924cf98e67/contentsharingsessions",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.contentSharingSession",
          "id": "F7D9EF30FF0A9BD3F64B274387FB8FF8E96B6CFBA8F87F8305A74DE99AF007BC"
        }
      ]
    }
  ]
}
```

#### Notification - content sharing updated

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/421f4c00-4436-4c3a-9d9a-c4924cf98e67/contentsharingsessions",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.contentSharingSession",
          "id": "F7D9EF30FF0A9BD3F64B274387FB8FF8E96B6CFBA8F87F8305A74DE99AF007BC"
        }
      ]
    }
  ]
}
```

#### Notification - content sharing ended

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/421f4c00-4436-4c3a-9d9a-c4924cf98e67/contentsharingsessions",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.contentSharingSession",
          "id": "F7D9EF30FF0A9BD3F64B274387FB8FF8E96B6CFBA8F87F8305A74DE99AF007BC"
        }
      ]
    }
  ]
}
```

Inherits from [entity](../resources/entity.md).

## Methods

| Method                                                                     | Return Type                                                  | Description                                                     |
|:---------------------------------------------------------------------------|:-------------------------------------------------------------|:----------------------------------------------------------------|
| [Get contentSharingSession](../api/contentsharingsession-get.md )          | [contentSharingSession](contentsharingsession.md)            | Retrieve the properties of a **contentSharingSession** object in a call.  |
| [List contentSharingSessions](../api/call-list-contentsharingsessions.md ) | [contentSharingSession](contentsharingsession.md) collection | Retrieve a list of **contentSharingSession** objects in a call. |


## Properties

| Property | Type   | Description                                                                                                    |
|:---------|:-------|:---------------------------------------------------------------------------------------------------------------|
| id       | String | Unique identifier for the content sharing session. Read-only. Inherited from [entity](../resources/entity.md). |

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.contentSharingSession"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.contentSharingSession",
  "id": "String (identifier)"
}
```
