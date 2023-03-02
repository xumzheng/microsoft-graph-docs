---
title: "localAdminPasswordSettings resource type"
description: "Represents settings for Azure AD local admin password solution (LAPS)"
author: "michaelrm97"
ms.localizationpriority: medium
ms.prod: "directory-management"
doc_type: resourcePageType
---
# localAdminPasswordSettings resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents settings for Azure AD local admin password solution (LAPS)

## Properties

|Property|Type|Description|
|:---|:---|:---|
|isEnabled|Boolean|Specified whether Azure AD LAPS is enabled or not for this tenant|

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.localAdminPasswordSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.localAdminPasswordSettings",
  "isEnabled": "Boolean",
}
```
