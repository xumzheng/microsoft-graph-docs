---
title: "accessPackageDirectoryRole resource type"
description: "A reference to a role defined in a directory role resource."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageDirectoryRole resource type

Namespace: microsoft.graph



A reference to a role defined in an [accessPackageDirectoryRoleResource](../resources/accesspackagedirectoryroleresource.md).

Inherits from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageDirectoryRoles](../api/accesspackagedirectoryrole-list.md)|[accessPackageDirectoryRole](../resources/accesspackagedirectoryrole.md) collection|Get a list of the [accessPackageDirectoryRole](../resources/accesspackagedirectoryrole.md) objects and their properties.|


## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentType|accessPackageDirectoryRoleAssignmentType|Indicates the type of directory role assignment that will be assigned.
The possible values are: `unknown`, `member`, `eligible`, `unknownFutureValue`.|
|description|String|A description for the resource role. Inherited from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).|
|displayName|String|The display name of the resource role such as the role defined by the application. Inherited from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).|
|id|String|Read-only. Inherited from [entity](../resources/entity.md).|
|roleId|String|The id of the role for the directory role resource.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[accessPackageResource](../resources/accesspackageresource.md)|**TODO: Add Description** Inherited from [microsoft.graph.accessPackageResourceRole](../resources/accesspackageresourcerole.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageDirectoryRole",
  "baseType": "microsoft.graph.accessPackageResourceRole",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageDirectoryRole",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "roleId": "String",
  "assignmentType": "String"
}
```

