---
title: "accessPackageResourceRequest resource type"
description: "An access package resource request is a request to a add a resource to a catalog so that the roles of the resource can be used in one or more of the catalog's access packages."
author: "saylee-dharne-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# accessPackageResourceRequest resource type

Namespace: microsoft.graph



In [Azure AD entitlement management](entitlementmanagement-overview.md), an access package resource request is a request to add a [resource](accesspackageresource.md) to a catalog so that the roles of the resource can be used in one or more of the catalog's access packages, or to remove a resource from a catalog that is no longer needed by the access packages.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageResourceRequests](../api/entitlementmanagement-list-resourcerequests.md)|[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) collection|Get a list of the [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects and their properties.|
|[Create accessPackageResourceRequest](../api/entitlementmanagement-post-resourcerequests.md)|[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)|Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The timestamp that this resource was created. The timestamp is in ISO 8601 formant and the time is always in UTC time.|
|id|String|Read-only. Inherited from [entity](../resources/entity.md).|
|requestType|accessPackageRequestType|The type of operation to be performed by the request.
The possible values are: `notSpecified`, `userAdd`, `userUpdate`, `userRemove`, `adminAdd`, `adminUpdate`, `adminRemove`, `systemAdd`, `systemUpdate`, `systemRemove`, `onBehalfAdd`, `unknownFutureValue`.|
|state|accessPackageRequestState|The current state of the request updated by the system.The possible values are: `submitted`, `pendingApproval`, `delivering`, `delivered`, `deliveryFailed`, `denied`, `scheduled`, `canceled`, `partiallyDelivered`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|catalog|[accessPackageCatalog](../resources/accesspackagecatalog.md)|The catalog associated with the resource request.|
|resource|[accessPackageResource](../resources/accesspackageresource.md)|The resource associated with the resource request.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceRequest",
  "id": "String (identifier)",
  "requestType": "String",
  "state": "String",
  "createdDateTime": "String (timestamp)"
}
```

