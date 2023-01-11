---
title: "Get recommendation"
description: "Read the properties and relationships of a recommendation object."
author: "hafowler"
ms.localizationpriority: medium
ms.prod: "identity-and-access"
doc_type: apiPageType
---

# Get recommendation
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [recommendation](../resources/recommendation.md) object.

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
GET /directory/recommendations/{recommendationId}
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

If successful, this method returns a `200 OK` response code and a [recommendation](../resources/recommendation.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "get_recommendation"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/recommendations/{recommendationId}
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.AAD.Reporting.recommendation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#Microsoft.AAD.Reporting.recommendation",
    "id": "bc2cb4cb-51af-e5b8-cbfc-3b48ee5306f2",
    "actionSteps": [
      {
        "@odata.type": "microsoft.graph.actionStep"
      }
    ],
    "benefits": "String",
    "category": "String",
    "createdDateTime": "String (timestamp)",
    "currentScore": "Double",
    "displayName": "String",
    "featureAreas": [
      "String"
    ],
    "impactType": "String",
    "impactStartDateTime": "String (timestamp)",
    "insights": "String",
    "lastCheckedDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)",
    "lastModifiedBy": "String",
    "maxScore": "Double",
    "postponeUntilDateTime": "String (timestamp)",
    "priority": "String",
    "status": "String",
    "remediationImpact": "String",
    "recommendationType": "String"
  }
}
```

