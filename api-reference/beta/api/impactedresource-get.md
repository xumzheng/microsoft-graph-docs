---
title: "Get impactedResource"
description: "Read the properties and relationships of an impactedResource object."
author: "hafowler"
ms.localizationpriority: medium
ms.prod: "identity-and-access"
doc_type: apiPageType
---

# Get impactedResource
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [impactedResource](../resources/impactedresource.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|DirectoryRecommendations.Read.All, DirectoryRecommendations.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|DirectoryRecommendations.Read.All, DirectoryRecommendations.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /directory/recommendations/{recommendationId}/impactedResources/{impactedResourceId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [impactedResource](../resources/impactedresource.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "get_impactedresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/recommendations/{recommendationId}/impactedResources/{impactedResourceId}
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
    "id": "5f0eaed8-2271-c706-a4db-7bc721c4eda4",
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

