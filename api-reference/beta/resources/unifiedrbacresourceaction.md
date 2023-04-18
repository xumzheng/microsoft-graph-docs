---
title: "unifiedRbacResourceAction resource type"
description: "Represents an operation that an authorized principal is allowed to perform."
author: "DougKirschner"
ms.localizationpriority: medium
ms.prod: "directory-management"
doc_type: resourcePageType
---

# unifiedRbacResourceAction resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents an operation that an authorized principal is allowed to perform.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List unifiedRbacResourceActions](../api/unifiedrbacresourcenamespace-list-resourceactions.md)|[unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) collection|Get a list of the [unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) objects and their properties.|
|[Get unifiedRbacResourceAction](../api/unifiedrbacresourceaction-get.md)|[unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md)|Read the properties and relationships of an [unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionVerb|String|HTTP method for the action, such as `DELETE`, `GET`, `PATCH`, `POST`, `PUT`, or `null`. Supports `$filter` (`eq`) but not for `null` values. |
|authenticationContextId|String|Conditional Access authentication context id that is assigned to the permission to add a protected action, such as `c1`. This property is only show when requested using `$select`.|
|description|String|Description for the action. Supports `$filter` (`eq`). |
|id|String|Unique identifier for an action within the resource namespace, such as `microsoft.insights-programs-update-patch`. Cannot include slash character (`/`). Case insensitive. Required. Supports `$filter` (`eq`). |
|isAuthenticationContextSettable|Boolean|This property indicates is the current resource can be assigned a Conditional Access authentication context .This property is only show when requested using `$select`.|
|name|String|Name for the action within the resource namespace, such as `microsoft.insights/programs/update`. Can include slash character (`/`). Case insensitive. Required. Supports `$filter` (`eq`). |
|resourceScopeId|String|Not implemented.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resourceActions|[unifiedRbacResourceAction](unifiedrbacresourceaction.md) collection|Operations that an authorized principal are allowed to perform.|
None.

<!-- The resourceScope relationship hasn't been implemented but is in the public schema. To unhide this and its related entities and methods once it's implemented.
|Relationship|Type|Description|
|:---|:---|:---|
|resourceScope| [unifiedRbacResourceScope](unifiedrbacresourcescope.md) |Not implemented.|
-->

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRbacResourceAction",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRbacResourceAction",
  "id": "String (identifier)",
  "actionVerb": "String",
  "description": "String",
  "name": "String",
  "resourceScopeId": "String"
}
```
