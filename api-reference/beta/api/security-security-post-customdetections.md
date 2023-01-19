---
title: "Create customDetection"
description: "Create a new microsoft.graph.security.customDetection object."
author: "mmekler"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: apiPageType
---

# Create customDetection
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [microsoft.graph.security.customDetection](../resources/security-customdetection.md) object.

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

**TODO: Remove properties that don't apply**
|Property|Type|Description|
|:---|:---|:---|
|ruleName|String|**TODO: Add Description** Required.|
|isEnabled|Boolean|**TODO: Add Description** Required.|
|frequency|String|**TODO: Add Description** Required.|
|createdBy|String|**TODO: Add Description** Optional.|
|creationDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|lastUpdatedBy|String|**TODO: Add Description** Optional.|
|lastQueryUpdateDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|lastRunDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|lastRunStatus|huntingRuleRunStatus|**TODO: Add Description**. The possible values are: `running`, `completed`, `failed`, `partiallyFailed`, `unknownFutureValue`. Optional.|
|lastRunFailureReason|String|**TODO: Add Description** Optional.|
|lastRunErrorCode|huntingRuleErrorCode|**TODO: Add Description**. The possible values are: `queryExecutionFailed`, `queryExecutionThrottling`, `queryExceededResultSize`, `queryLimitsExceeded`, `queryTimeout`, `alertCreationFailed`, `alertReportNotFound`, `partialRowsFailed`, `unknownFutureValue`. Optional.|
|nextRunDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|queryText|String|**TODO: Add Description** Required.|
|alertTitle|String|**TODO: Add Description** Required.|
|alertDescription|String|**TODO: Add Description** Required.|
|alertSeverity|alertSeverity|**TODO: Add Description**. The possible values are: `unknown`, `informational`, `low`, `medium`, `high`, `unknownFutureValue`. Required.|
|alertCategory|String|**TODO: Add Description** Required.|
|mitreTechniques|String collection|**TODO: Add Description** Optional.|
|alertRecommendedAction|String|**TODO: Add Description** Optional.|
|organizationalScope|String collection|**TODO: Add Description** Optional.|
|serviceSources|serviceSource collection|**TODO: Add Description**. The possible values are: `unknown`, `microsoftDefenderForEndpoint`, `microsoftDefenderForIdentity`, `microsoftDefenderForCloudApps`, `microsoftDefenderForOffice365`, `microsoft365Defender`, `azureAdIdentityProtection`, `microsoftAppGovernance`, `dataLossPrevention`, `unknownFutureValue`. Required.|
|impactedEntities|[microsoft.graph.security.customDetectionImpactedEntity](../resources/security-customdetectionimpactedentity.md) collection|**TODO: Add Description** Required.|
|actions|[microsoft.graph.security.customDetectionAction](../resources/security-customdetectionaction.md) collection|**TODO: Add Description** Optional.|



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

