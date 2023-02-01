---
title: "accessPackageAuthorizationScope resource type"
description: "A reference to a scope within an authorization resource."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageAuthorizationScope resource type

Namespace: microsoft.graph



A reference to a scope within an[accessPackageAuthorizationResource](../resources/accesspackageauthorizationresource.md).

Inherits from [accessPackageResourceScope](../resources/accesspackageresourcescope.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageAuthorizationScopes](../api/accesspackageauthorizationscope-list.md)|[accessPackageAuthorizationScope](../resources/accesspackageauthorizationscope.md) collection|Get a list of the [accessPackageAuthorizationScope](../resources/accesspackageauthorizationscope.md) objects and their properties.|
|[Get accessPackageAuthorizationScope](../api/accesspackageauthorizationscope-get.md)|[accessPackageAuthorizationScope](../resources/accesspackageauthorizationscope.md)|Read the properties and relationships of an [accessPackageAuthorizationScope](../resources/accesspackageauthorizationscope.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|*The description of the scope. Inherited from [accessPackageResourceScope](../resources/accesspackageresourcescope.md).|
|displayName|String|The display name of the scope. Inherited from [accessPackageResourceScope](../resources/accesspackageresourcescope.md).|
|id|String|Read-only. Inherited from [entity](../resources/entity.md).|
|isRootScope|Boolean|True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource. Inherited from [accessPackageResourceScope](../resources/accesspackageresourcescope.md).|
|scopeId|String|The id of the scope within the authorization resource|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[accessPackageResource](../resources/accesspackageresource.md)|The resource that this scope is associated with. |

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAuthorizationScope",
  "baseType": "microsoft.graph.accessPackageResourceScope",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAuthorizationScope",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isRootScope": "Boolean",
  "scopeId": "String"
}
```

