---
title: "accessPackageDefaultScope resource type"
description: "The default scope of an access package resource."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageDefaultScope resource type

Namespace: microsoft.graph



The default scope of an access package resource.

Inherits from [accessPackageResourceScope](../resources/accesspackageresourcescope.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageDefaultScopes](../api/accesspackagedefaultscope-list.md)|[accessPackageDefaultScope](../resources/accesspackagedefaultscope.md) collection|Get a list of the [accessPackageDefaultScope](../resources/accesspackagedefaultscope.md) objects and their properties.|
|[Get accessPackageDefaultScope](../api/accesspackagedefaultscope-get.md)|[accessPackageDefaultScope](../resources/accesspackagedefaultscope.md)|Read the properties and relationships of an [accessPackageDefaultScope](../resources/accesspackagedefaultscope.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|The description of the scope. Inherited from [accessPackageResourceScope](../resources/accesspackageresourcescope.md).|
|displayName|String|The display name of the scope. Inherited from [accessPackageResourceScope](../resources/accesspackageresourcescope.md).|
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
  "@odata.type": "microsoft.graph.accessPackageDefaultScope",
  "baseType": "microsoft.graph.accessPackageResourceScope",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageDefaultScope",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isRootScope": "Boolean"
}
```

