---
title: "profileVideoMetadata resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: resourcePageType
---

# profileVideoMetadata resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [itemFacet](../resources/itemfacet.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List profileVideoMetadatas](../api/profile-list-profilevideometadata.md)|[profileVideoMetadata](../resources/profilevideometadata.md) collection|Get a list of the [profileVideoMetadata](../resources/profilevideometadata.md) objects and their properties.|
|[Create profileVideoMetadata](../api/profile-post-profilevideometadata.md)|[profileVideoMetadata](../resources/profilevideometadata.md)|Create a new [profileVideoMetadata](../resources/profilevideometadata.md) object.|
|[Get profileVideoMetadata](../api/profilevideometadata-get.md)|[profileVideoMetadata](../resources/profilevideometadata.md)|Read the properties and relationships of a [profileVideoMetadata](../resources/profilevideometadata.md) object.|
|[Update profileVideoMetadata](../api/profilevideometadata-update.md)|[profileVideoMetadata](../resources/profilevideometadata.md)|Update the properties of a [profileVideoMetadata](../resources/profilevideometadata.md) object.|
|[Delete profileVideoMetadata](../api/profile-delete-profilevideometadata.md)|None|Delete a [profileVideoMetadata](../resources/profilevideometadata.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedAudiences|allowedAudiences|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md).The possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/intune-identityset.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md).|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|inference|[inferenceData](../resources/inferencedata.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md).|
|isSearchable|Boolean|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/intune-identityset.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md).|
|profileVideoUrl|String|**TODO: Add Description**|
|source|[personDataSources](../resources/persondatasources.md)|**TODO: Add Description** Inherited from [itemFacet](../resources/itemfacet.md).|

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

