---
title: "accessPackagePowerPlatformRole resource type"
description: "A reference to a role defined in an accessPackagePowerPlatformResource"
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackagePowerPlatformRole resource type

Namespace: microsoft.graph



A reference to a role defined in an [accessPackagePowerPlatformResource](../resources/accesspackagepowerplatformresource.md).

Inherits from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackagePowerPlatformRoles](../api/accesspackagepowerplatformrole-list.md)|[accessPackagePowerPlatformRole](../resources/accesspackagepowerplatformrole.md) collection|Get a list of the [accessPackagePowerPlatformRole](../resources/accesspackagepowerplatformrole.md) objects and their properties.|


## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|A description for the resource role. Inherited from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).|
|displayName|String|The display name of the resource role such as the role defined by the application. Inherited from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).|
|groupId|String|The group id.|
|id|String|Read-only. Inherited from [entity](../resources/entity.md).|
|powerPlatformRoleType|accessPackagePowerPlatformRoleType|Indicates the type of power platform role that will be assigned. The possible values are: `unknown`, `security`, `ownerTeam`, `securityGroupTeam`, `microsoft365GroupTeam`, `canvasAppOwner`, `canvasAppUser`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[accessPackageResource](../resources/accesspackageresource.md)|The resource that this role is associated with. Inherited from [microsoft.graph.accessPackageResourceRole](../resources/accesspackageresourcerole.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackagePowerPlatformRole",
  "baseType": "microsoft.graph.accessPackageResourceRole",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackagePowerPlatformRole",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "groupId": "String",
  "powerPlatformRoleType": "String"
}
```

