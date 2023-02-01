---
title: "accessPackageResourceRoleScope resource type"
description: "**TODO: Add Description**"
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageResourceRoleScope resource type

Namespace: microsoft.graph



In [Azure AD entitlement management](entitlementmanagement-overview.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource for that scope.  An access package will have access package resource role scopes for the resources in its catalog which are relevant to that access package.  When a subject receives an access package assignment, the subject will be provisioned with the role in that scope of each access package resource role scope.

Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageResourceRoleScopes](../api/accesspackage-list-resourcerolescopes.md)|[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) collection|Get a list of the [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects and their properties.|
|[Create accessPackageResourceRoleScope](../api/accesspackage-post-resourcerolescopes.md)|[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)|Create a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.|
|[Get accessPackageResourceRoleScope](../api/accesspackageresourcerolescope-get.md)|[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)|Read the properties and relationships of an [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.|
|[Delete accessPackageResourceRoleScope](../api/accesspackage-delete-resourcerolescopes.md)|None|Delete an [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The timestamp that this resource was created. The timestamp is in ISO 8601 formant and the time is always in UTC time.|
|id|String| Read-only. Inherited from [entity](../resources/entity.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|role|[accessPackageResourceRole](../resources/accesspackageresourcerole.md)|The resource role associated with the role scope. Read-only. Supports `$expand`.|
|scope|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|The resource scope associated with the role scope. Read-only. Supports `$expand`.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceRoleScope",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)"
}
```

