---
title: "accessPackageApplicationRole resource type"
description: "A reference to a role defined in a service principal resource"
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageApplicationRole resource type

Namespace: microsoft.graph



A reference to a role defined in an [accessPackageServicePrincipalResource](../resources/accesspackageserviceprincipalresource.md).

Inherits from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageApplicationRoles](../api/accesspackageapplicationrole-list.md)|[accessPackageApplicationRole](../resources/accesspackageapplicationrole.md) collection|Get a list of the [accessPackageApplicationRole](../resources/accesspackageapplicationrole.md) objects and their properties.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appRoleId|String|The id of the role in the application.|
|description|String|A description for the resource role. Inherited from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).|
|displayName|String|The display name of the resource role such as the role defined by the application. Inherited from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).|
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
  "@odata.type": "microsoft.graph.accessPackageApplicationRole",
  "baseType": "microsoft.graph.accessPackageResourceRole",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageApplicationRole",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "appRoleId": "String"
}
```

