---
title: "recommendation: postpone"
description: "Postpone action on a recommendation object to a specified future date and time."
author: "hafowler"
ms.localizationpriority: medium
ms.prod: "identity-and-access"
doc_type: apiPageType
---

# recommendation: postpone
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Postpone action on a [recommendation](../resources/recommendation.md) object to a specified future date and time by marking its **status** as `postponed`. On the date and time provided, Azure AD will automatically update the **status** of the **recommendation** object to `active` again.

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
POST /directory/recommendations/{recommendationId}/postpone
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
|postponeUntilDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [recommendation](../resources/recommendation.md) in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "recommendationthis.postpone"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/recommendations/{recommendationId}/postpone
Content-Type: application/json

{
  "postponeUntilDateTime": "String (timestamp)"
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

