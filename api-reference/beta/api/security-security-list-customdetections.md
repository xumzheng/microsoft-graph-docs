---
title: "List customDetections"
description: "Get a list of the microsoft.graph.security.customDetection objects and their properties."
author: "mmekler"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: apiPageType
---

# List customDetections
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [microsoft.graph.security.customDetection](../resources/security-customdetection.md) objects and their properties.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged)               |
|:---------------------------------------|:----------------------------------------------------------|
| Delegated (work or school account)     | CustomDetections.Read.All, CustomDetections.ReadWrite.All |
| Delegated (personal Microsoft account) | Not supported.                                            |
| Application                            | CustomDetections.Read.All, CustomDetections.ReadWrite.All |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/customDetections
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

If successful, this method returns a `200 OK` response code and a collection of [customDetection](../resources/security-customdetection.md) objects in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "list_customdetection"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/customDetections
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.customDetection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.security.customDetection",
      "id": "11315927-7a96-cbb4-93b1-371676cbcdd7",
      "ruleName": "String",
      "isEnabled": "Boolean",
      "frequency": "String",
      "createdBy": "String",
      "creationDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)",
      "lastUpdatedBy": "String",
      "lastQueryUpdateDateTime": "String (timestamp)",
      "lastRunDateTime": "String (timestamp)",
      "lastRunStatus": "String",
      "lastRunFailureReason": "String",
      "lastRunErrorCode": "String",
      "nextRunDateTime": "String (timestamp)",
      "queryText": "String",
      "alertTitle": "String",
      "alertDescription": "String",
      "alertSeverity": "String",
      "alertCategory": "String",
      "mitreTechniques": [
        "String"
      ],
      "alertRecommendedAction": "String",
      "organizationalScope": [
        "String"
      ],
      "serviceSources": [
        "String"
      ],
      "impactedEntities": [
        {
          "@odata.type": "microsoft.graph.security.customDetectionImpactedEntity"
        }
      ],
      "actions": [
        {
          "@odata.type": "microsoft.graph.security.customDetectionAction"
        }
      ]
    }
  ]
}
```

