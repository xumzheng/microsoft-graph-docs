---
title: "recommendation: dismiss"
description: "Dismiss a recommendation object and updates its status to dismissed."
author: "hafowler"
ms.localizationpriority: medium
ms.prod: "identity-and-access"
doc_type: apiPageType
---

# recommendation: dismiss
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Dismiss a [recommendation](../resources/recommendation.md) object that you consider to be inapplicable to your directory and update its **status** to `dismissed` .

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
POST /directory/recommendations/{recommendationId}/dismiss
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
|dismissReason|String|Explanation for why this recommendation is not applicable to your directory.|



## Response

If successful, this action returns a `200 OK` response code and a [recommendation](../resources/recommendation.md) in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "recommendationthis.dismiss"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/recommendations/{recommendationId}/dismiss
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
  "@odata.type": "Microsoft.AAD.Reporting.recommendation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#Microsoft.AAD.Reporting.recommendation",
    "id": "String (identifier)",
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

