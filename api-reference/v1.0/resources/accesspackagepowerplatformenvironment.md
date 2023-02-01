---
title: "accessPackagePowerPlatformEnvironment resource type"
description: "The environment of a power platform resource"
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackagePowerPlatformEnvironment resource type

Namespace: microsoft.graph


The environment of a [power platform resource](../resources/accesspackagepowerplatformresource.md).


Inherits from [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackagePowerPlatformEnvironments](../api/accesspackagepowerplatformenvironment-list.md)|[accessPackagePowerPlatformEnvironment](../resources/accesspackagepowerplatformenvironment.md) collection|Get a list of the [accessPackagePowerPlatformEnvironment](../resources/accesspackagepowerplatformenvironment.md) objects and their properties.|
|[Get accessPackagePowerPlatformEnvironment](../api/accesspackagepowerplatformenvironment-get.md)|[accessPackagePowerPlatformEnvironment](../resources/accesspackagepowerplatformenvironment.md)|Read the properties and relationships of an [accessPackagePowerPlatformEnvironment](../resources/accesspackagepowerplatformenvironment.md) object.|


## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationUrl|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|The date and time that this object was created. <br>The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.|
|description|String|A description of environment.|
|displayName|String|The display name of the environment.|
|environmentId|String|**TODO: Add Description**|
|id|String|The system-assigned unique identifier of the object. Inherited from [entity](../resources/entity.md).|
|isDefaultEnvironment|Boolean|Determines whether this is default environment or not. It is set to `true` for all static origin systems, such as Azure AD groups and Azure AD Applications.|
|modifiedDateTime|DateTimeOffset|The date and time that this object was last modified. <br>The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resources|[accessPackageResource](../resources/accesspackageresource.md) collection|The resources associated with the environment. Read-only. Required.Inherited from [microsoft.graph.accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackagePowerPlatformEnvironment",
  "baseType": "microsoft.graph.accessPackageResourceEnvironment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackagePowerPlatformEnvironment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isDefaultEnvironment": "Boolean",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "environmentId": "String",
  "applicationUrl": "String"
}
```

