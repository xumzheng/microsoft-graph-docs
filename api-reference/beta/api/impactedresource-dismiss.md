---
title: "impactedResource: dismiss"
description: "Dismiss a recommendationResource object and update its status to dismissed."
author: "hafowler"
ms.localizationpriority: medium
ms.prod: "identity-and-access"
doc_type: apiPageType
---

# impactedResource: dismiss
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Dismiss an [impactedResources](../resources/impactedresource.md) object and update its status to `dismissed`.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|DirectoryRecommendations.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|DirectoryRecommendations.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /directory/recommendations/{recommendationId}/impactedResources/{impactedResourceId}/dismiss
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|dismissReason|String|Audited reason for deeming an [impactedResource](../resources/impactedresource.md) inapplicable to you and its associated [recommendation](../resources/recommendation.md).|



## Response

If successful, this action returns a `200 OK` response code and a [impactedResource](../resources/impactedresource.md) in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "impactedresourcethis.dismiss"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/recommendations/{recommendationId}/impactedResources/{impactedResourceId}/dismiss
Content-Type: application/json

{
  "dismissReason": "String"
}
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.AAD.Reporting.impactedResource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#Microsoft.AAD.Reporting.impactedResource",
    "id": "String (identifier)",
    "subjectId": "String",
    "recommendationId": "String",
    "addedDateTime": "String (timestamp)",
    "portalUrl": "String",
    "apiUrl": "String",
    "displayName": "String",
    "resourceType": "String",
    "owner": "String",
    "rank": "Integer",
    "status": "String",
    "additionalDetails": [
      {
        "@odata.type": "microsoft.graph.keyValue"
      }
    ],
    "lastModifiedBy": "String",
    "lastModifiedDateTime": "String",
    "postponeUntilDateTime": "String (timestamp)"
  }
}
```

