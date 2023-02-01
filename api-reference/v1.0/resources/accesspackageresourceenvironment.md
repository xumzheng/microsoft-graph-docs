---
title: "accessPackageResourceEnvironment resource type"
description: "A reference to the geolocation environment in which a resource is located"
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageResourceEnvironment resource type

Namespace: microsoft.graph


In [Azure AD Entitlement Management](entitlementmanagement-overview.md), an access package resource environment is a reference to the geolocation environment in which a resource is located. This environment is automatically provided as part of Azure AD Entitlement Management. The API is only applicable to resources for non-static origin systems.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageResourceEnvironments](../api/accesspackagepowerplatformresource-list-environment.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) collection|Get a list of the [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects and their properties.|
|[Get accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Read the properties and relationships of an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time that this object was created. <br>The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.|
|description|String|A description of environment.|
|displayName|String|The display name of the environment.|
|id|String|The system-assigned unique identifier of the object. Inherited from [entity](../resources/entity.md).|
|isDefaultEnvironment|Boolean|Determines whether this is default environment or not. It is set to `true` for all static origin systems, such as Azure AD groups and Azure AD Applications.|
|modifiedDateTime|DateTimeOffset|The date and time that this object was last modified. <br>The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resources|[accessPackageResource](../resources/accesspackageresource.md) collection|The resources associated with the environment. Read-only. Required.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceEnvironment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceEnvironment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isDefaultEnvironment": "Boolean",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)"
}
```

