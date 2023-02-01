---
title: "accessPackageResourceRole resource type"
description: "A reference to a role defined in a resource"
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageResourceRole resource type

Namespace: microsoft.graph



In [Azure AD entitlement management](entitlementmanagement-overview.md), an access package resource role is a reference to a role defined in a resource. These are automatically present after [a resource is added to an access package catalog](../api/entitlementmanagement-post-accesspackageresourcerequests.md). That reference can be used after creating an access package to specify the roles of each of the catalog's resources into which an access package should deliver, by [creating an access package resource role scope](../api/accesspackage-post-accesspackageresourcerolescopes.md).

Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageResourceRoles](../api/accesspackageresource-list-roles.md)|[accessPackageResourceRole](../resources/accesspackageresourcerole.md) collection|Get a list of the [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects and their properties.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|A description for the resource role.|
|displayName|String|The display name of the resource role such as the role defined by the application.|
|id|String|Read-only. Inherited from [entity](../resources/entity.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[accessPackageResource](../resources/accesspackageresource.md)|The resource that this role is associated with. |

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceRole",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```

