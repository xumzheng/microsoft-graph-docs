---
title: "notificationChannel resource type"
description: "Include information about an alert rule's notification channels selected by user."
author: "zhishending"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: resourcePageType
---

# notificationChannel resource type

Namespace: microsoft.graph.deviceManagement

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Include information about an alert rule's notification channels selected by user.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|notificationChannelType|notificationChannelType|Type of notification channel.The possible values are: `portal`, `email`, `phoneCall`, `sms`, `unknownFutureValue`.|
|receivers|String collection|Contact information of notification receivers, like email addresses. For portal notification, receivers can be left blank. For email notification, receivers consist of email addresses like foo@bar.com|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagement.notificationChannel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement.notificationChannel",
  "notificationChannelType": "String",
  "receivers": [
    "String"
  ]
}
```
