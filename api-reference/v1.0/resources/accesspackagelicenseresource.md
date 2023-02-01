---
title: "accessPackageLicenseResource resource type"
description: "A reference to a license resource."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageLicenseResource resource type

Namespace: microsoft.graph



A reference to a [license resource](../resources/licensedetails.md).


Inherits from [accessPackageResource](../resources/accesspackageresource.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageLicenseResources](../api/accesspackagelicenseresource-list.md)|[accessPackageLicenseResource](../resources/accesspackagelicenseresource.md) collection|Get a list of the [accessPackageLicenseResource](../resources/accesspackagelicenseresource.md) objects and their properties.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attributes|[accessPackageResourceAttribute](../resources/accesspackageresourceattribute.md) collection|Contains information about the attributes to be collected from the requestor and sent to the resource application. Inherited from [accessPackageResource](../resources/accesspackageresource.md).|
|createdDateTime|DateTimeOffset|The timestamp that the resource was added. The timestamp is in ISO 8601 format in UTC time. Inherited from [accessPackageResource](../resources/accesspackageresource.md).|
|description|String|A description for the resource.Inherited from [accessPackageResource](../resources/accesspackageresource.md).|
|displayName|String|he display name of the resource, such as the application name, group name, or site name. Inherited from [accessPackageResource](../resources/accesspackageresource.md).|
|id|String|Read-only. Inherited from [entity](../resources/entity.md).|
|modifiedDateTime|DateTimeOffset|The timestamp that this resource was last modified. The timestamp is in ISO 8601 format in UTC time. Read-only. Inherited from [accessPackageResource](../resources/accesspackageresource.md).|
|skuId|String|The license sku id.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|environment|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)| Contains the environment information for the resource. Supports `$expand`. Inherited from [microsoft.graph.accessPackageResource](../resources/accesspackageresource.md)|
|roles|[accessPackageResourceRole](../resources/accesspackageresourcerole.md) collection| Read-only. Nullable. Supports `$expand`. Inherited from [microsoft.graph.accessPackageResource](../resources/accesspackageresource.md)|
|scopes|[accessPackageResourceScope](../resources/accesspackageresourcescope.md) collection| Read-only. Nullable. Supports `$expand`. Inherited from [microsoft.graph.accessPackageResource](../resources/accesspackageresource.md)|



## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageLicenseResource",
  "baseType": "microsoft.graph.accessPackageResource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageLicenseResource",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "attributes": [
    {
      "@odata.type": "microsoft.graph.accessPackageResourceAttribute"
    }
  ],
  "skuId": "String"
}
```

