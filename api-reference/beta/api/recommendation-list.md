---
title: "List recommendations"
description: "Get a list of the recommendation objects and their properties."
author: "hafowler"
ms.localizationpriority: medium
ms.prod: "identity-and-access"
doc_type: apiPageType
---

# List recommendationBases
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [recommendation](../resources/recommendation.md) objects and their properties.

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
GET /directory/recommendations
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

If successful, this method returns a `200 OK` response code and a collection of [recommendationBase](../resources/recommendationbase.md) objects in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "list_recommendationbase"
}
-->
``` http
GET https://graph.microsoft.com/beta/directory/recommendations
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.AAD.Reporting.recommendation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.AAD.Reporting.recommendation",
      "id": "2a6b89e0-bc33-9bce-229c-0b9058a9bfe2",
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
  ]
}
```

