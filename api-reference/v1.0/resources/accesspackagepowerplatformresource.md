---
title: "accessPackagePowerPlatformResource resource type"
description: "A reference to a Microsoft power platform resource."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackagePowerPlatformResource resource type

Namespace: microsoft.graph



A reference to a Microsoft power platform resource.

Inherits from [accessPackageResource](../resources/accesspackageresource.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackagePowerPlatformResources](../api/accesspackagepowerplatformresource-list.md)|[accessPackagePowerPlatformResource](../resources/accesspackagepowerplatformresource.md) collection|Get a list of the [accessPackagePowerPlatformResource](../resources/accesspackagepowerplatformresource.md) objects and their properties.|


## Properties
|Property|Type|Description|
|:---|:---|:---|
|attributes|[accessPackageResourceAttribute](../resources/accesspackageresourceattribute.md) collection|Contains information about the attributes to be collected from the requestor and sent to the resource application. Inherited from [accessPackageResource](../resources/accesspackageresource.md).|
|createdDateTime|DateTimeOffset|The timestamp that the resource was added. The timestamp is in ISO 8601 format in UTC time. Inherited from [accessPackageResource](../resources/accesspackageresource.md).|
|description|String|A description for the resource.Inherited from [accessPackageResource](../resources/accesspackageresource.md).|
|displayName|String|he display name of the resource, such as the application name, group name, or site name. Inherited from [accessPackageResource](../resources/accesspackageresource.md).|
|id|String|Read-only. Inherited from [entity](../resources/entity.md).|
|modifiedDateTime|DateTimeOffset|The timestamp that this resource was last modified. The timestamp is in ISO 8601 format in UTC time. Read-only. Inherited from [accessPackageResource](../resources/accesspackageresource.md).|
|powerAppId|String|The id of the power app.|
|powerPlatformResourceType|accessPackagePowerPlatformResourceType|The type of power platform resource. The possible values are: `unknown`, `businessUnit`, `powerApp`, `unknownFutureValue`.|

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
  "@odata.type": "microsoft.graph.accessPackagePowerPlatformResource",
  "baseType": "microsoft.graph.accessPackageResource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackagePowerPlatformResource",
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
  "powerAppId": "String",
  "powerPlatformResourceType": "String"
}
```

