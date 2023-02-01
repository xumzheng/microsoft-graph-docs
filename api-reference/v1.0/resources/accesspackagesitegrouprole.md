---
title: "accessPackageSiteGroupRole resource type"
description: "A reference to a role defined in an accessPackageSharePointResource"
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageSiteGroupRole resource type

Namespace: microsoft.graph



A reference to a role defined in an [accessPackageSharePointResource](../resources/accesspackagesharepointresource.md.

Inherits from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageSiteGroupRoles](../api/accesspackagesitegrouprole-list.md)|[accessPackageSiteGroupRole](../resources/accesspackagesitegrouprole.md) collection|Get a list of the [accessPackageSiteGroupRole](../resources/accesspackagesitegrouprole.md) objects and their properties.|


## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|A description for the resource role. Inherited from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).|
|displayName|String|The display name of the resource role such as the role defined by the application. Inherited from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).|
|groupId|String|The site group id.|
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
  "@odata.type": "microsoft.graph.accessPackageSiteGroupRole",
  "baseType": "microsoft.graph.accessPackageResourceRole",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageSiteGroupRole",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "groupId": "String"
}
```

