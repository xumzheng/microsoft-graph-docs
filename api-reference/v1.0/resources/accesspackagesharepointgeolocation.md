---
title: "accessPackageSharePointGeoLocation resource type"
description: "**TODO: Add Description**"
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageSharePointGeoLocation resource type

Namespace: microsoft.graph

The geolocation of a SharePoint Online site for a [accessPackageSharePointResource](../resources/accesspackagesharepointresource.md).


Inherits from [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageSharePointGeoLocations](../api/accesspackagesharepointgeolocation-list.md)|[accessPackageSharePointGeoLocation](../resources/accesspackagesharepointgeolocation.md) collection|Get a list of the [accessPackageSharePointGeoLocation](../resources/accesspackagesharepointgeolocation.md) objects and their properties.|
|[Get accessPackageSharePointGeoLocation](../api/accesspackagesharepointgeolocation-get.md)|[accessPackageSharePointGeoLocation](../resources/accesspackagesharepointgeolocation.md)|Read the properties and relationships of an [accessPackageSharePointGeoLocation](../resources/accesspackagesharepointgeolocation.md) object.|


## Properties
|Property|Type|Description|
|:---|:---|:---|
|adminUrl|String|The admin url of the sharepoint geo-location.|
|createdDateTime|DateTimeOffset|The date and time that this object was created. <br>The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.|
|description|String|A description of environment.|
|displayName|String|The display name of the environment.|
|id|String|The system-assigned unique identifier of the object. Inherited from [entity](../resources/entity.md).|
|isDefaultEnvironment|Boolean|Determines whether this is default environment or not. It is set to `true` for all static origin systems, such as Azure AD groups and Azure AD Applications.|
|modifiedDateTime|DateTimeOffset|The date and time that this object was last modified. <br>The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resources|[accessPackageResource](../resources/accesspackageresource.md) collection|The resources associated with the environment. Inherited from [microsoft.graph.accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageSharePointGeoLocation",
  "baseType": "microsoft.graph.accessPackageResourceEnvironment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageSharePointGeoLocation",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isDefaultEnvironment": "Boolean",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "adminUrl": "String"
}
```

