---
title: "accessPackageLicenseRole resource type"
description: "A reference to a role defined in an accessPackageLicenseResource."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageLicenseRole resource type

Namespace: microsoft.graph



A reference to a role defined in an [accessPackageLicenseResource](../resources/accesspackagelicenseresource.md).

Inherits from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageLicenseRoles](../api/accesspackagelicenserole-list.md)|[accessPackageLicenseRole](../resources/accesspackagelicenserole.md) collection|Get a list of the [accessPackageLicenseRole](../resources/accesspackagelicenserole.md) objects and their properties.|


## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|A description for the resource role. Inherited from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).|
|displayName|String|The display name of the resource role such as the role defined by the application. Inherited from [accessPackageResourceRole](../resources/accesspackageresourcerole.md).|
|id|String|Read-only. Inherited from [entity](../resources/entity.md).|
|skuId|String|The license sku id.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[accessPackageResource](../resources/accesspackageresource.md)|The resource that this role is associated with. Inherited from [microsoft.graph.accessPackageResourceRole](../resources/accesspackageresourcerole.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageLicenseRole",
  "baseType": "microsoft.graph.accessPackageResourceRole",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageLicenseRole",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "skuId": "String"
}
```

