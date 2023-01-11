---
title: "impactedResource: postpone"
description: "Postpone action on an impactedResource object to a specified future date and time."
author: "hafowler"
ms.localizationpriority: medium
ms.prod: "identity-and-access"
doc_type: apiPageType
---

# impactedResource: postpone
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Postpone action on an [impactedResource](../resources/impactedresource.md) object to a specified future date and time by marking its **status** as `postponed`. On the specified date and time, Azure AD will automatically mark the status of the **impactedResource** object to `active`.

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
POST /directory/recommendations/{recommendationId}/impactedResources/{impactedResourceId}/postpone
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
|postponeUntilDateTime|DateTimeOffset|The date and time when the **status** of the **impactedResource** will be updated to `active`.|



## Response

If successful, this action returns a `200 OK` response code and a [impactedResource](../resources/impactedresource.md) in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "impactedresourcethis.postpone"
}
-->
``` http
POST https://graph.microsoft.com/beta/directory/recommendations/{recommendationId}/impactedResources/{impactedResourceId}/postpone
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

