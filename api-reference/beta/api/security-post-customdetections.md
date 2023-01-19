---
title: "Create customDetection"
description: "Create a new customDetection object."
author: "mmekler"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: apiPageType
---

# Create customDetection
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new customDetection object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
|:---------------------------------------|:--------------------------------------------|
| Delegated (work or school account)     | CustomDetections.ReadWrite.All              |
| Delegated (personal Microsoft account) | Not supported.                              |
| Application                            | CustomDetections.ReadWrite.All              |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/customDetections
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [microsoft.graph.security.customDetection](../resources/security-customdetection.md) object.

You can specify the following properties when creating a **customDetection**.

| Property               | Type                                                                                                                        | Description                                                                                                                                                                          |
|:-----------------------|:----------------------------------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ruleName               | String                                                                                                                      | Name of the custom detection rule.                                                                                                                                                   |
| isEnabled              | Boolean                                                                                                                     | Indicates whether custom detection is turned on for the tenant.                                                                                                                      |
| frequency              | String                                                                                                                      | How often the detection rule is set to run.                                                                                                                                          |
| queryText              | String                                                                                                                      | Contents of the query.                                                                                                                                                               |
| alertTitle             | String                                                                                                                      | Name of the alert triggered by the custom detection rule.                                                                                                                            |
| alertDescription       | String                                                                                                                      | Description of the alert triggered by the custom detection rule.                                                                                                                     |
| alertSeverity          | alertSeverity                                                                                                               | Severity assigned to the alert triggered by the custom detection rule. The possible values are: `unknown`, `informational`, `low`, `medium`, `high`, `unknownFutureValue`. Required. |
| alertCategory          | String                                                                                                                      | Category assigned to the alert triggered by the custom detection rule.                                                                                                               |
| mitreTechniques        | String collection                                                                                                           | MITRE technique assigned to the alert triggered by the custom detection rule.                                                                                                        |
| alertRecommendedAction | String                                                                                                                      | Recommended actions to mitigate the threat related to the alert triggered by the custom detection rule.                                                                              |
| organizationalScope    | String collection                                                                                                           | List of device groups to which the custom detection rule applies.                                                                                                                    |
| impactedEntities       | [microsoft.graph.security.customDetectionImpactedEntity](../resources/security-customdetectionimpactedentity.md) collection | Which entity or entities were impacted based on the alert triggered by the custom detection rule.                                                                                    |
| actions                | [microsoft.graph.security.customDetectionAction](../resources/security-customdetectionaction.md) collection                 | Actions taken on impacted entities as set in the custom detection rule.                                                                                                              |

## Response

If successful, this method returns a `201 Created` response code and a [microsoft.graph.security.customDetection](../resources/security-customdetection.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "create_customdetection_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/customDetections
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.security.customDetection",
  "ruleName": "String",
  "isEnabled": "Boolean",
  "frequency": "String",
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
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.customDetection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

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
```

