---
title: "accessPackageGroupResource resource type"
description: "A reference to an Azure AD group resource."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageGroupResource resource type

Namespace: microsoft.graph



A reference to an [Azure AD group](../resource/group.md) resource.


Inherits from [accessPackageResource](../resources/accesspackageresource.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageGroupResources](../api/accesspackagegroupresource-list.md)|[accessPackageGroupResource](../resources/accesspackagegroupresource.md) collection|Get a list of the [accessPackageGroupResource](../resources/accesspackagegroupresource.md) objects and their properties.|


## Properties
|Property|Type|Description|
|:---|:---|:---|
|attributes|[accessPackageResourceAttribute](../resources/accesspackageresourceattribute.md) collection|Contains information about the attributes to be collected from the requestor and sent to the resource application. Inherited from [accessPackageResource](../resources/accesspackageresource.md).|
|createdDateTime|DateTimeOffset|The timestamp that the resource was added. The timestamp is in ISO 8601 format in UTC time. Inherited from [accessPackageResource](../resources/accesspackageresource.md).|
|description|String|A description for the resource.Inherited from [accessPackageResource](../resources/accesspackageresource.md).|
|displayName|String|he display name of the resource, such as the application name, group name, or site name. Inherited from [accessPackageResource](../resources/accesspackageresource.md).|
|groupId|String|The id of the group.|
|groupType|accessPackageGroupType|The type of group. The possible values are: `unknown`, `security`, `unified`, `teams`, `assignableToRole`, `mailEnabled`, `distribution`, `dynamicMembership`, `unknownFutureValue`.|
|id|String|Read-only. Inherited from [entity](../resources/entity.md).|
|modifiedDateTime|DateTimeOffset|The timestamp that this resource was last modified. The timestamp is in ISO 8601 format in UTC time. Read-only. Inherited from [accessPackageResource](../resources/accesspackageresource.md).|

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
  "@odata.type": "microsoft.graph.accessPackageGroupResource",
  "baseType": "microsoft.graph.accessPackageResource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageGroupResource",
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
  "groupId": "String",
  "groupType": "String"
}
```

