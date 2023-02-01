---
title: "accessPackageResourceScope resource type"
description: "In Azure AD entitlement management, an access package resource scope is a reference to a scope within a resource."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageResourceScope resource type

Namespace: microsoft.graph



In [Azure AD entitlement management](entitlementmanagement-overview.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.

You can determine the access package resource scope, for a resource which has roles already added to an access package, by using [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) to return a collection of [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) objects.

If the resource is in an access package catalog but has not yet had its roles added to an access package, you can determine the access package resource scope by using [list accessPackageResources](../api/accesspackagecatalog-list-accesspackageresources.md) and including `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` in the query.

Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageResourceScopes](../api/accesspackagepowerplatformresource-list-scopes.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md) collection|Get a list of the [accessPackageResourceScope](../resources/accesspackageresourcescope.md) objects and their properties.|
|[Get accessPackageResourceScope](../api/accesspackageresourcescope-get.md)|[accessPackageResourceScope](../resources/accesspackageresourcescope.md)|Read the properties and relationships of an [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|The description of the scope.|
|displayName|String|The display name of the scope.|
|id|String|Read-only. Inherited from [entity](../resources/entity.md).|
|isRootScope|Boolean|True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[accessPackageResource](../resources/accesspackageresource.md)|The resource that this scope is associated with. |

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceScope",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceScope",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isRootScope": "Boolean"
}
```

