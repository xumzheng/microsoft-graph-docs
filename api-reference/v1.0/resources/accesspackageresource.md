---
title: "accessPackageResource resource type"
description: ""An access package resource is a reference to a resource associated with a catalog the roles for which can be used in one or more access packages."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageResource resource type

Namespace: microsoft.graph


In [Azure AD Entitlement Management](entitlementmanagement-overview.md), an access package resource is a reference to a resource associated with an access package catalog. The roles for the access package resource can be used in one or more access packages.  To request to associate a resource with an access package catalog, or remove a resource from a catalog, create an [accessPackageResourceRequest](accesspackageresourcerequest.md).


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageResources](../api/accesspackagecatalog-list-resources.md)|[accessPackageResource](../resources/accesspackageresource.md) collection|Get a list of the [accessPackageResource](../resources/accesspackageresource.md) objects and their properties.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attributes|[accessPackageResourceAttribute](../resources/accesspackageresourceattribute.md) collection| Contains information about the attributes to be collected from the requestor and sent to the resource application. |
|createdDateTime|DateTimeOffset|The timestamp that the resource was added. The timestamp is in ISO 8601 format in UTC time.  |
|description|String|A description for the resource.|
|displayName|String|The display name of the resource, such as the application name, group name, or site name. |
|id|String|Read-only.|
|modifiedDateTime|DateTimeOffset|The timestamp that this resource was last modified. The timestamp is in ISO 8601 format in UTC time. Read-only.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|environment|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Contains the environment information for the resource. This can be set with an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) using either the `@odata.bind` annotation or by linking to the related environment using the id of the environment. Supports `$expand`.|
|roles|[accessPackageResourceRole](../resources/accesspackageresourcerole.md) collection|Read-only. Nullable. Supports `$expand`.|
|scopes|[accessPackageResourceScope](../resources/accesspackageresourcescope.md) collection|Read-only. Nullable. Supports `$expand`.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResource",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "attributes": [
    {
      "@odata.type": "microsoft.graph.accessPackageResourceAttribute"
    }
  ]
}
```

