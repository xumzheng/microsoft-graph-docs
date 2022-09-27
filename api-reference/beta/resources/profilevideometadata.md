---
title: "profileVideoMetadata resource type"
description: "Represents metadata of a user's profile video"
author: "kevinbellinger"
ms.localizationpriority: medium
ms.prod: "people"
doc_type: resourcePageType
---

# profileVideoMetadata resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents metadata for the user's profile video, which helps access, play and manage the video.


This resource type inherits from [itemFacet](../resources/itemfacet.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get profileVideoMetadata](../api/profilevideometadata-get.md)|[profileVideoMetadata](../resources/profilevideometadata.md)|Read the properties and relationships of a [profileVideoMetadata](../resources/profilevideometadata.md) object.|
|[Update profileVideoMetadata](../api/profilevideometadata-update.md)|[profileVideoMetadata](../resources/profilevideometadata.md)|Update the properties of a [profileVideoMetadata](../resources/profilevideometadata.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedAudiences|allowedAudiences|The audiences that are able to see the values contained within the entity. Inherited from [itemFacet](../resources/itemfacet.md).The possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/intune-identityset.md)|Provides the identifier of the user and/or application that created the entity. Inherited from [itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Provides the dateTimeOffset for when the entity was created. Inherited from [itemFacet](../resources/itemfacet.md).|
|id|String|Identifier used for individually addressing the entity. Inherited from [entity](../resources/entity.md).|
|inference|[inferenceData](../resources/inferencedata.md)|Contains inference detail if the entity is inferred by the creating or modifying application. Inherited from [itemFacet](../resources/itemfacet.md).|
|isSearchable|Boolean|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/intune-identityset.md)|Provides the identifier of the user and/or application that last modified the entity. Inherited from [itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Provides the dateTimeOffset for when the entity was created. Inherited from [itemFacet](../resources/itemfacet.md).|
|profileVideoUrl|String|Provides the url to the actual profile video file|
|source|[personDataSources](../resources/persondatasources.md)|Where the values originated if synced from another service. Inherited from [itemFacet](../resources/itemfacet.md).|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profileVideoMetadata",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.profileVideoMetadata",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSources"
  },
  "isSearchable": "Boolean",
  "profileVideoUrl": "String"
}
```

