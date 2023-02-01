---
title: "accessPackageGroupRole resource type"
description: "A reference to a role defined for an Azure AD group."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageGroupRole resource type

Namespace: microsoft.graph



A reference to a role defined in for an [accessPackageGroupResource](../resources/accesspackagegroupresource.md).

Inherits from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageGroupRoles](../api/accesspackagegrouprole-list.md)|[accessPackageGroupRole](../resources/accesspackagegrouprole.md) collection|Get a list of the [accessPackageGroupRole](../resources/accesspackagegrouprole.md) objects and their properties.|


## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|A description for the resource role. Inherited from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).|
|displayName|String|The display name of the resource role such as the role defined by the application. Inherited from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).|
|groupId|String|The group id. |
|groupMemberType|accessPackageGroupMemberType|Indicates the type of group membership that will be assigned via the role. The possible values are: `unknown`, `member`, `owner`, `unknownFutureValue`.|
|id|String|Read-only. Inherited from [entity](../resources/entity.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[accessPackageResource](../resources/accesspackageresource.md)|The resource that this role is associated with. Inherited from [microsoft.graph.accessPackageResourceRole](../resources/accesspackageresourcerole.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageGroupRole",
  "baseType": "microsoft.graph.accessPackageResourceRole",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageGroupRole",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "groupId": "String",
  "groupMemberType": "String"
}
```

